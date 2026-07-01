# .NET MAUI Developer Roadmap

[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](http://makeapullrequest.com)
[![License: CC BY-NC-SA 4.0](https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc-sa/4.0/)

Roadmap to becoming a [.NET MAUI](https://learn.microsoft.com/en-us/dotnet/maui/) developer in 2026.

Below you can find a chart demonstrating the paths that you can take and the libraries you would want to learn to become a .NET MAUI developer. It is meant as a tip for everyone who asks, "What should I learn next as a mobile & desktop .NET developer?"

> ⚠️ **Coming from Xamarin?** Xamarin reached **end of support on May 1, 2024**. .NET MAUI is its direct successor and the framework you should be learning today. This roadmap is the modernized version of the classic [Xamarin Developer Roadmap](https://github.com/Stayrony/Xamarin-Developer-Roadmap). Most of your Xamarin knowledge (C#, XAML, MVVM, platform concepts) carries over — see Microsoft's [Xamarin → .NET MAUI migration guide](https://learn.microsoft.com/en-us/dotnet/maui/migration/).

## Disclaimer

> The purpose of this roadmap is to give you an idea about the landscape. It will guide you if you are confused about what to learn next, rather than encouraging you to pick what is hip and trendy. You should grow some understanding of *why* one tool would be better suited for some cases than another — and remember that hip and trendy does not always mean best suited for the job.

## Give a Star! ⭐

If you like or are using this project to learn or start your solution, please give it a star. Thanks!

## Roadmap

![Roadmap](./maui-developer-roadmap.png)

> An editable mind-map is available in [`maui-developer-roadmap.xmind`](./maui-developer-roadmap.xmind) (open with [XMind](https://xmind.app/)).

## Resources

### 1. Learn the Prerequisites

- [C#](https://learn.microsoft.com/en-us/dotnet/csharp/) — the language of the entire .NET ecosystem
- [.NET fundamentals](https://learn.microsoft.com/en-us/dotnet/fundamentals/) — the SDK, `dotnet` CLI, project files (SDK-style `.csproj`), NuGet
- Understand the difference between **.NET** (the unified platform, currently .NET 9 / .NET 10) and the legacy .NET Framework

### 2. General Development Skills

- Learn **Git**, create a few repositories on GitHub, share your code with other people
- Know the **HTTP(S)** protocol, request methods (GET, POST, PUT, PATCH, DELETE, OPTIONS)
- Don't be afraid of using search engines and AI coding assistants — but verify what they tell you
- Learn the basics of **CI/CD**
- Application settings & configuration (`appsettings.json`, secrets, environment-specific config)
- Read a few books about algorithms and data structures

### 3. C#

- [Language fundamentals](https://learn.microsoft.com/en-us/dotnet/csharp/) — types, generics, records
- [async / await](https://learn.microsoft.com/en-us/dotnet/csharp/asynchronous-programming/) — non-blocking UI is essential on mobile
- [LINQ](https://learn.microsoft.com/en-us/dotnet/csharp/linq/)
- [Nullable reference types](https://learn.microsoft.com/en-us/dotnet/csharp/nullable-references) & modern C# features

### 4. XAML

- [Data bindings](https://learn.microsoft.com/en-us/dotnet/maui/fundamentals/data-binding/) & [compiled bindings](https://learn.microsoft.com/en-us/dotnet/maui/fundamentals/data-binding/compiled-bindings) (prefer compiled bindings for performance)
- [Triggers](https://learn.microsoft.com/en-us/dotnet/maui/fundamentals/triggers)
- [Behaviors](https://learn.microsoft.com/en-us/dotnet/maui/fundamentals/behaviors)
- [Markup extensions](https://learn.microsoft.com/en-us/dotnet/maui/xaml/markup-extensions/) & [C# Markup](https://learn.microsoft.com/en-us/dotnet/communitytoolkit/maui/markup/markup)
- [Control Templates](https://learn.microsoft.com/en-us/dotnet/maui/fundamentals/controltemplate) & [Data Templates](https://learn.microsoft.com/en-us/dotnet/maui/fundamentals/datatemplate)
- [Accessibility](https://learn.microsoft.com/en-us/dotnet/maui/fundamentals/accessibility)
- [**Handlers**](https://learn.microsoft.com/en-us/dotnet/maui/user-interface/handlers/) — lightweight, decoupled way to customize and extend native controls in MAUI
- The new **XAML source generator** (.NET 10) creates strongly-typed code for XAML at compile time

### 5. .NET MAUI Fundamentals

- [What is .NET MAUI](https://learn.microsoft.com/en-us/dotnet/maui/what-is-maui) — one project targeting Android, iOS, macOS (Mac Catalyst), and Windows (WinUI 3)
- [Single project structure](https://learn.microsoft.com/en-us/dotnet/maui/fundamentals/single-project) — one `.csproj`, multi-targeted; shared resources, fonts, images
- [App lifecycle](https://learn.microsoft.com/en-us/dotnet/maui/fundamentals/app-lifecycle)
- [Layouts](https://learn.microsoft.com/en-us/dotnet/maui/user-interface/layouts/) (Grid, StackLayout, FlexLayout, AbsoluteLayout)
- [**Shell**](https://learn.microsoft.com/en-us/dotnet/maui/fundamentals/shell/) — flyout, tabs, and URI-based navigation
- [**.NET MAUI Essentials**](https://learn.microsoft.com/en-us/dotnet/maui/platform-integration/) — device APIs (sensors, connectivity, geolocation, preferences, secure storage) built directly into the framework
- [Platform-specific code](https://learn.microsoft.com/en-us/dotnet/maui/platform-integration/invoke-platform-code) — partial classes, `#if ANDROID/IOS/...`, `Platforms/` folders
- [Hot Reload](https://learn.microsoft.com/en-us/dotnet/maui/xaml/hot-reload) (XAML) and .NET Hot Reload (C#)
  1. **Android**
      - [Android project structure & manifest](https://learn.microsoft.com/en-us/dotnet/maui/android/)
      - Activities, Intents, permissions
  2. **iOS & Mac Catalyst**
      - [iOS project structure](https://learn.microsoft.com/en-us/dotnet/maui/ios/), `Info.plist`, entitlements
      - Understanding App Delegate / Scene lifecycle
  3. **Windows (WinUI 3)**
      - [Windows project structure](https://learn.microsoft.com/en-us/dotnet/maui/windows/), packaging (MSIX)

### 6. UI Controls & Interaction

- [Controls gallery](https://learn.microsoft.com/en-us/dotnet/maui/user-interface/controls/) — buttons, entries, pickers, etc.
- [**CollectionView**](https://learn.microsoft.com/en-us/dotnet/maui/user-interface/controls/collectionview/) & [CarouselView](https://learn.microsoft.com/en-us/dotnet/maui/user-interface/controls/carouselview/) — modern, performant lists
- [BindableLayout](https://learn.microsoft.com/en-us/dotnet/maui/user-interface/layouts/bindablelayout) — bind a layout to a collection
- [Building custom controls](https://learn.microsoft.com/en-us/dotnet/maui/user-interface/controls/contentview) (ContentView, bindable properties, templated controls)
- [**Gestures**](https://learn.microsoft.com/en-us/dotnet/maui/fundamentals/gestures/) — tap, swipe, pan, pinch, drag & drop
- [**Animations**](https://learn.microsoft.com/en-us/dotnet/maui/user-interface/animation/basic) — basic & easing animations
- [Popups, toasts & snackbars](https://learn.microsoft.com/en-us/dotnet/communitytoolkit/maui/alerts/) (CommunityToolkit.Maui)

### 7. Styling & Theming

- [Styles (XAML)](https://learn.microsoft.com/en-us/dotnet/maui/user-interface/styles/xaml) — explicit, implicit, and `BasedOn` styles
- [**Resource Dictionaries**](https://learn.microsoft.com/en-us/dotnet/maui/fundamentals/resource-dictionaries) & merged dictionaries
- [Dynamic resources](https://learn.microsoft.com/en-us/dotnet/maui/user-interface/styles/xaml#dynamic-styles)
- [**Dark / light theme**](https://learn.microsoft.com/en-us/dotnet/maui/user-interface/system-theme-changes) — `AppThemeBinding` and responding to system theme changes
- [Visual states](https://learn.microsoft.com/en-us/dotnet/maui/user-interface/visual-states) (VisualStateManager)
- [Platform-specific styling](https://learn.microsoft.com/en-us/dotnet/maui/platform-integration/customize-ui-appearance) (OnPlatform, OnIdiom)

### 8. Resources: Fonts, Images & App Icons

- [Images](https://learn.microsoft.com/en-us/dotnet/maui/user-interface/images/images) — adding, sizing, and multi-resolution assets
- [**Fonts & font icons**](https://learn.microsoft.com/en-us/dotnet/maui/user-interface/fonts) — embedding custom fonts, using icon fonts
- [**App icons**](https://learn.microsoft.com/en-us/dotnet/maui/user-interface/images/app-icons) — adaptive, single-source SVG
- [**Splash screen**](https://learn.microsoft.com/en-us/dotnet/maui/user-interface/images/splashscreen)
- [Raw & embedded assets](https://learn.microsoft.com/en-us/dotnet/maui/user-interface/images/rawfiles)

### 9. MVVM Fundamentals

- [MVVM pattern](https://learn.microsoft.com/en-us/dotnet/architecture/maui/mvvm)
- [**Dependency Injection**](https://learn.microsoft.com/en-us/dotnet/maui/fundamentals/dependency-injection) — built into MAUI via `Microsoft.Extensions.DependencyInjection`; register services in `MauiProgram.cs`
- [Navigation](https://learn.microsoft.com/en-us/dotnet/maui/fundamentals/shell/navigation) — Shell routing & query parameters
- [Commands](https://learn.microsoft.com/en-us/dotnet/maui/fundamentals/data-binding/commanding) — prefer `[RelayCommand]` from CommunityToolkit.Mvvm
- [Converters](https://learn.microsoft.com/en-us/dotnet/maui/fundamentals/data-binding/converters)
- [Validation](https://learn.microsoft.com/en-us/dotnet/architecture/maui/validation)
- **Messaging**: use [`WeakReferenceMessenger`](https://learn.microsoft.com/en-us/dotnet/communitytoolkit/mvvm/messenger) (CommunityToolkit.Mvvm) for decoupled component communication

### 10. MVVM / App Frameworks

- [**CommunityToolkit.Mvvm**](https://learn.microsoft.com/en-us/dotnet/communitytoolkit/mvvm/) — **recommended default.** Observable properties and commands with minimal boilerplate via source generators (`[ObservableProperty]`, `[RelayCommand]`)
- [**.NET MAUI Community Toolkit**](https://learn.microsoft.com/en-us/dotnet/communitytoolkit/maui/) — controls, converters, behaviors, `MediaElement`, popups. Remember to call `.UseMauiCommunityToolkit()` in `MauiProgram.cs`
- [Prism](https://prismlibrary.com/) — full-featured app framework (modularity, navigation, dialogs) with MAUI support
- [ReactiveUI](https://reactiveui.net/) — composable, reactive (Rx) MVVM framework
- [MVVMCross](https://www.mvvmcross.com/) — mature cross-platform MVVM framework

### 11. App Architecture

- [MAUI enterprise app patterns](https://learn.microsoft.com/en-us/dotnet/architecture/maui/) — Microsoft's reference architecture (eShop)
- [Clean Architecture](https://learn.microsoft.com/en-us/dotnet/architecture/modern-web-apps-azure/common-web-application-architectures#clean-architecture) — separation of concerns, dependency rule
- Project & folder structure, feature-based organization
- Sharing code across projects (Core/domain layer, `.NET Standard`/shared libraries)
- State management & the repository/service patterns

### 12. Blazor Hybrid

- [Blazor Hybrid](https://learn.microsoft.com/en-us/aspnet/core/blazor/hybrid/) — build UI with Razor components running in a `BlazorWebView`, sharing code with your web app
- [.NET MAUI Blazor apps](https://learn.microsoft.com/en-us/dotnet/maui/user-interface/controls/blazorwebview)
- Great for teams with existing web/Blazor skills and shared web + native codebases

### 13. API Clients

1. **REST**
    - [Refit](https://github.com/reactiveui/refit) — automatic type-safe REST library
    - [Flurl](https://flurl.dev/) — fluent, testable URL builder + HTTP client
    - [RestSharp](https://restsharp.dev/) — simple REST/HTTP client
    - [`IHttpClientFactory`](https://learn.microsoft.com/en-us/dotnet/core/extensions/httpclient-factory) — the recommended way to configure/consume `HttpClient`
    - [Polly](https://github.com/App-vNext/Polly) / [Microsoft.Extensions.Http.Resilience](https://learn.microsoft.com/en-us/dotnet/core/resilience/) — retries, circuit breakers, timeouts
2. **GraphQL**
    - [Strawberry Shake](https://chillicream.com/docs/strawberryshake) — strongly-typed GraphQL client for .NET
    - [GraphQL.Client](https://github.com/graphql-dotnet/graphql-client)

### 14. Data Access

1. **Local databases**
    - [SQLite-net](https://github.com/praeclarum/sqlite-net) — lightweight ORM over SQLite
    - [EF Core](https://learn.microsoft.com/en-us/ef/core/) — full-featured ORM, works with SQLite on-device
    - [LiteDB](https://www.litedb.org/) — a .NET NoSQL document store in a single file
2. **Device storage** (built into MAUI Essentials)
    - [Preferences](https://learn.microsoft.com/en-us/dotnet/maui/platform-integration/storage/preferences) — key/value settings
    - [Secure Storage](https://learn.microsoft.com/en-us/dotnet/maui/platform-integration/storage/secure-storage) — encrypted key/value (Keychain / Keystore)
    - [File system helpers](https://learn.microsoft.com/en-us/dotnet/maui/platform-integration/storage/file-system-helpers)
3. **Caching**
    - [Akavache](https://github.com/reactiveui/Akavache) — async key/value store
    - [MonkeyCache](https://github.com/jamesmontemagno/monkey-cache) — simple caching library
4. **Cloud / Backend**
    - [Firebase](https://firebase.google.com/docs) (Firestore, Realtime Database)
    - [Supabase](https://supabase.com/docs/reference/csharp/introduction) — open-source Postgres backend with a C# client
    - [Azure Mobile Apps / Datasync](https://learn.microsoft.com/en-us/azure/developer/mobile-apps/azure-mobile-apps/overview) — offline sync

### 15. Authentication

- [Biometric authentication](https://learn.microsoft.com/en-us/dotnet/communitytoolkit/maui/) — fingerprint / Face ID / Touch ID (via community plugins such as Plugin.Fingerprint)
- [**WebAuthenticator**](https://learn.microsoft.com/en-us/dotnet/maui/platform-integration/communication/authentication) — built-in OAuth browser flow (MAUI Essentials)
- [MSAL.NET](https://learn.microsoft.com/en-us/entra/identity-platform/msal-net-migration) — Microsoft Entra ID / Azure AD authentication
- **Social sign-in**: Google, Apple, Facebook, Microsoft (via OAuth/OIDC + WebAuthenticator)
- [Sign in with Apple](https://learn.microsoft.com/en-us/dotnet/maui/platform-integration/communication/authentication) — required by Apple if you offer other social logins
- OpenID Connect libraries: [IdentityModel.OidcClient](https://github.com/IdentityModel/IdentityModel.OidcClient)

### 16. Security

- [Secure Storage](https://learn.microsoft.com/en-us/dotnet/maui/platform-integration/storage/secure-storage) — never store secrets in plain preferences
- [**OWASP MASVS**](https://mas.owasp.org/) — the mobile app security verification standard
- **Certificate / SSL pinning** — protect against MITM attacks
- Root / jailbreak detection
- Code protection — [trimming](https://learn.microsoft.com/en-us/dotnet/core/deploying/trimming/trim-self-contained) & obfuscation
- Secrets management — keep API keys out of source; use a backend proxy where possible

### 17. Media

- [MediaElement](https://learn.microsoft.com/en-us/dotnet/communitytoolkit/maui/views/mediaelement) (CommunityToolkit.Maui) — audio/video playback
- [Media picker & camera](https://learn.microsoft.com/en-us/dotnet/maui/platform-integration/device-media/picker) — built into MAUI Essentials
- [SkiaSharp](https://github.com/mono/SkiaSharp) — 2D graphics engine
- [`GraphicsView` + Microsoft.Maui.Graphics](https://learn.microsoft.com/en-us/dotnet/maui/user-interface/graphics/) — cross-platform drawing
- [Lottie animations](https://github.com/Baseflow/LottieXamarin) / SkiaSharp.Skottie — vector animations

### 18. Maps & Location

- [Map control](https://learn.microsoft.com/en-us/dotnet/maui/user-interface/controls/map) (`Microsoft.Maui.Controls.Maps`) — pins, polygons, map types
- [Geolocation](https://learn.microsoft.com/en-us/dotnet/maui/platform-integration/device/geolocation) — current position & continuous updates (MAUI Essentials)
- [Geocoding](https://learn.microsoft.com/en-us/dotnet/maui/platform-integration/device/geocoding) — address ↔ coordinates
- Geofencing (via platform APIs)

### 19. Real-Time Communication

- [SignalR](https://learn.microsoft.com/en-us/aspnet/core/signalr/) — real-time server → client messaging
- [gRPC](https://learn.microsoft.com/en-us/aspnet/core/grpc/) — high-performance RPC (including gRPC-Web)

### 20. Logging

- [Microsoft.Extensions.Logging](https://learn.microsoft.com/en-us/dotnet/core/extensions/logging) — the built-in logging abstraction (register in `MauiProgram.cs`)
- [Serilog](https://serilog.net/) — structured logging
- [NLog](https://nlog-project.org/) — flexible logging platform

### 21. Testing

1. [Unit Testing](https://learn.microsoft.com/en-us/dotnet/core/testing/)
    - [xUnit](https://xunit.net/) — popular .NET unit-testing framework
    - [NUnit](https://nunit.org/) — long-standing unit-testing framework
    - [TUnit](https://github.com/thomhurst/TUnit) — modern, source-generated test framework
2. **Mocking**
    - [Moq](https://github.com/devlooped/moq) — mocking library
    - [NSubstitute](https://nsubstitute.github.io/) — friendly mocking library
3. **Behavior (BDD)**
    - [Reqnroll](https://reqnroll.net/) — BDD framework using the Gherkin specification language
4. **UI / E2E Testing**
    - [Appium](https://appium.io/) — cross-platform UI automation (the recommended path for MAUI E2E testing)
    - [.NET MAUI UITest samples](https://github.com/dotnet/maui/tree/main/src/Controls/tests/TestCases.Shared.Tests)
5. **Blazor Hybrid testing**
    - [bUnit](https://bunit.dev/) — testing Razor components

### 22. Crash Reporting & Analytics

- [Sentry](https://docs.sentry.io/platforms/dotnet/guides/maui/) — crash reporting & performance monitoring with first-class MAUI support
- [Firebase Crashlytics](https://firebase.google.com/docs/crashlytics) & [Firebase Analytics](https://firebase.google.com/docs/analytics)
- [Azure Application Insights](https://learn.microsoft.com/en-us/azure/azure-monitor/app/app-insights-overview) — telemetry & analytics

### 23. Payment Gateway

- [In-app purchases (iOS) / In-app billing (Android)](https://github.com/jamesmontemagno/InAppBillingPlugin) — Plugin.InAppBilling
- [Apple Pay](https://developer.apple.com/apple-pay/) & [Google Pay](https://developers.google.com/pay/api)
- [Stripe](https://stripe.com/docs) — online payment processing
- [Braintree](https://developer.paypal.com/braintree/docs) / PayPal
- [Adyen](https://docs.adyen.com/) — global payment platform

### 24. Push Notifications

1. **Remote**
    - [Firebase Cloud Messaging (FCM)](https://firebase.google.com/docs/cloud-messaging) — cross-platform push
    - [Azure Notification Hubs](https://learn.microsoft.com/en-us/azure/notification-hubs/notification-hubs-push-notification-overview)
    - [Plugin.Firebase](https://github.com/TobiasBuchholz/Plugin.Firebase) — MAUI-friendly Firebase wrapper
2. **Local**
    - [Plugin.LocalNotification](https://github.com/thudugala/Plugin.LocalNotification) — cross-platform local notifications

### 25. Background Work

- Platform background models — Android [foreground services](https://developer.android.com/develop/background-work/services/foreground-services) & [WorkManager](https://developer.android.com/develop/background-work/background-tasks), iOS [BGTaskScheduler](https://developer.apple.com/documentation/backgroundtasks)
- Long-running tasks & scheduled/periodic work
- [Plugin.Maui.TaskScheduler](https://github.com/jfversluis) and similar community plugins
- Keeping work alive across app suspension/termination

### 26. Artificial Intelligence (AI)

1. **On-device ML**
    - [ONNX Runtime](https://onnxruntime.ai/) — run ML models cross-platform on-device
    - [ML Kit](https://developers.google.com/ml-kit) (Android) / [Core ML](https://developer.apple.com/documentation/coreml) (iOS)
2. **LLMs & Generative AI**
    - [Microsoft.Extensions.AI](https://learn.microsoft.com/en-us/dotnet/ai/microsoft-extensions-ai) — unified AI abstractions for .NET
    - [Semantic Kernel](https://learn.microsoft.com/en-us/semantic-kernel/) — orchestrate LLMs, plugins, and agents
    - [Azure AI / Azure OpenAI](https://learn.microsoft.com/en-us/azure/ai-services/) and [OpenAI .NET SDK](https://github.com/openai/openai-dotnet)
3. **Augmented Reality**
    - [ARCore](https://developers.google.com/ar) (Android) / [ARKit](https://developer.apple.com/augmented-reality/) (iOS) via platform bindings
4. **OCR / Vision**
    - [ML Kit Text Recognition](https://developers.google.com/ml-kit/vision/text-recognition), [Azure AI Vision](https://azure.microsoft.com/en-us/products/ai-services/ai-vision), [Google Cloud Vision](https://cloud.google.com/vision)
    - [Tesseract](https://github.com/tesseract-ocr/tesseract) — open-source OCR engine

### 27. Advertising

- [Google AdMob](https://admob.google.com/home/) — via community plugins (e.g. Plugin.MauiMTAdmob)
- [AppLovin MAX](https://www.applovin.com/max/) / other mediation platforms

### 28. App Distribution

1. **Android** — [Publish to Google Play](https://learn.microsoft.com/en-us/dotnet/maui/android/deployment/publish-google-play) (AAB), [Amazon Appstore](https://developer.amazon.com/apps-and-games)
2. **iOS** — [Publish to the App Store](https://learn.microsoft.com/en-us/dotnet/maui/ios/deployment/publish-app-store) via App Store Connect
3. **Windows** — [Publish to the Microsoft Store](https://learn.microsoft.com/en-us/dotnet/maui/windows/deployment/publish-cli) (MSIX)
4. **macOS** — [Publish a Mac Catalyst app](https://learn.microsoft.com/en-us/dotnet/maui/mac-catalyst/deployment/publish-app-store)
5. Beta testing: [TestFlight](https://developer.apple.com/testflight/) (iOS), [Google Play internal testing](https://support.google.com/googleplay/android-developer/answer/9845334)

### 29. CI/CD

- [GitHub Actions](https://learn.microsoft.com/en-us/dotnet/maui/deployment/) — build/test/sign MAUI apps
- [Azure DevOps Pipelines](https://learn.microsoft.com/en-us/azure/devops/pipelines/)
- [`dotnet publish`](https://learn.microsoft.com/en-us/dotnet/maui/deployment/) for automated builds per platform
- Code signing & provisioning (fastlane for iOS/Android is still widely used)

### 30. Advanced

1. **Native interop**
    - [Android binding libraries](https://learn.microsoft.com/en-us/dotnet/android/binding-libs/) (Java/Kotlin)
    - [iOS binding libraries](https://learn.microsoft.com/en-us/dotnet/ios/binding-libs/) (Objective-C/Swift)
    - [Native library interop](https://learn.microsoft.com/en-us/dotnet/maui/platform-integration/native-library-interop) — Slim Bindings
2. **Cross-platform**
    - [Deep linking / App links](https://learn.microsoft.com/en-us/dotnet/maui/) & Shell URI navigation
    - [Localization](https://learn.microsoft.com/en-us/dotnet/maui/fundamentals/localization)
    - [Performance](https://learn.microsoft.com/en-us/dotnet/maui/deployment/performance) — startup tracing, layout diagnostics (.NET 10), **trimming & NativeAOT** for iOS/Mac Catalyst

### 31. Tools

- [Visual Studio 2022](https://visualstudio.microsoft.com/) (Windows) with the .NET MAUI workload
- [Visual Studio Code](https://code.visualstudio.com/) + the [.NET MAUI extension](https://marketplace.visualstudio.com/items?itemName=ms-dotnettools.dotnet-maui) — cross-platform, including macOS
- [JetBrains Rider](https://www.jetbrains.com/rider/) — strong MAUI support
- [`dotnet` CLI](https://learn.microsoft.com/en-us/dotnet/core/tools/) — build, run, publish from the terminal
- [Postman](https://www.postman.com/) — test web-service requests/responses
- [Proxyman](https://proxyman.io/) / [Charles](https://www.charlesproxy.com/) — HTTP(S) traffic inspection

### 32. Game Engine

- [MonoGame](https://monogame.net/) — free C# framework for cross-platform games
- For richer needs, a dedicated engine like [Godot](https://godotengine.org/) (C# support) or Unity is the practical choice

### 33. SOLID

- [Single Responsibility Principle (SRP)](https://en.wikipedia.org/wiki/Single-responsibility_principle)
- [Open-Closed Principle (OCP)](https://en.wikipedia.org/wiki/Open%E2%80%93closed_principle)
- [Liskov Substitution Principle (LSP)](https://en.wikipedia.org/wiki/Liskov_substitution_principle)
- [Interface Segregation Principle (ISP)](https://en.wikipedia.org/wiki/Interface_segregation_principle)
- [Dependency Inversion Principle (DIP)](https://en.wikipedia.org/wiki/Dependency_inversion_principle)

### 34. Design Patterns

- [Abstract Factory](https://refactoring.guru/design-patterns/abstract-factory)
- [Factory Method](https://refactoring.guru/design-patterns/factory-method)
- [Command](https://refactoring.guru/design-patterns/command)
- [Decorator](https://refactoring.guru/design-patterns/decorator)
- [Strategy](https://refactoring.guru/design-patterns/strategy)
- [Observer](https://refactoring.guru/design-patterns/observer)
- [Builder](https://refactoring.guru/design-patterns/builder)
- [Singleton](https://refactoring.guru/design-patterns/singleton)
- [Facade](https://refactoring.guru/design-patterns/facade)
- [Mediator](https://refactoring.guru/design-patterns/mediator)

## Wrap Ups

If you think the roadmap can be improved, please open a PR with any updates and submit any issues. This is a living document — star the repository to revisit.

Migrating an existing Xamarin app? Start with Microsoft's [Xamarin → .NET MAUI migration guide](https://learn.microsoft.com/en-us/dotnet/maui/migration/).

Inspired by the original [Xamarin Developer Roadmap](https://github.com/Stayrony/Xamarin-Developer-Roadmap) and the [ASP.NET Core Developer Roadmap](https://github.com/MoienTajik/AspNetCore-Developer-Roadmap).

## Contribution

Want to contribute? We encourage community feedback and contributions. Please follow our [contributing guidelines](./CONTRIBUTING.md).

## License

[![License: CC BY-NC-SA 4.0](https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc-sa/4.0/)
