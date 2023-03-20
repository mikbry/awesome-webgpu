# Awesome WebGPU [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> Lovely curated list of WebGPU resources, libraries and tools.

[WebGPU](https://en.wikipedia.org/wiki/WebGPU) is a work in progress [Web standard from W3C](https://www.w3.org/TR/webgpu/) for modern 3D and GPU computing. Its purpose is to get the best performances on recent GPUs from desktop to mobile. Unlike WebGL, WebGPU is not a port of an existing native API. It borrows concepts from Metal, Vulkan and Direct3D12.

## Contents

- [Websites](#websites)
- [Browser support](#browser-support)
- [Articles](#articles)
- [Tutorials](#tutorials)
- [Books](#books)
- [Libraries](#libraries)
- [Gists](#gists)
- [Demos](#demos)
- [Videos](#videos)
- [Presentations](#presentations)
- [Community](#community)
- [Bug reporting](#bug-reporting)
- [Contribute](#contribute)
- [License](#license)

## Websites

- [GPU for the Web Community Group](https://webgpu.io) - Official website
- [GPUWeb](https://github.com/gpuweb/gpuweb) - Official Github repository
- [WebGPU - Twitter](https://twitter.com/webgpu) - Official Twitter account
- Official WebGPU Specifications: [Working Draft](https://www.w3.org/TR/webgpu/) / [Editor's Draft](https://gpuweb.github.io/gpuweb/)
- Official WGSL (WebGPU Shading Language) Specifications: [Working Draft](https://www.w3.org/TR/WGSL/) / [Editor's Draft](https://gpuweb.github.io/gpuweb/wgsl/)
- [Official WebGPU Explainer](https://gpuweb.github.io/gpuweb/explainer/)
- [API quick reference and documentation](https://webgpu.rocks/) - WebGPU.rocks
- [107 WebGPU Projects on GitHub](https://awesomeopensource.com/projects/webgpu) - AwesomeOpenSource.com
- [r/WebGPU - Reddit](https://www.reddit.com/r/webgpu/) - WebGPU Subreddit

## Browser support

- [Implementation status](https://github.com/gpuweb/gpuweb/wiki/Implementation-Status) - Official W3C Group
- [Register for Google Chrome origin trial](https://developer.chrome.com/origintrials/#/view_trial/118219490218475521) - Chrome Developers
- [WebGPU browser support overview](https://caniuse.com/webgpu) - CanIUse.com
- [Chrome Platform Status](https://www.chromestatus.com/feature/6213121689518080) - Chrome Developers
- [WebGPU and WSL in Safari](https://webkit.org/blog/9528/webgpu-and-wsl-in-safari/) - WebKit
- [WebGPU on iOS](https://mil-tokyo.github.io/webdnn/docs/tips/enable_webgpu_ios.html) - Don't work on my iPhone6+
- [Servo MVP](https://github.com/servo/servo/projects/24) - WebGPU MVP

### Try out WebGPU

- Chromium ([Chrome Canary](https://www.google.com/chrome/canary/), [Edge Canary](https://www.microsoftedgeinsider.com/download/canary), ...): Go to `about:flags#enable-unsafe-webgpu` and enable the "Unsafe WebGPU" flag.
- [Firefox Nightly](https://nightly.mozilla.org/): Go to `about:config` and set `dom.webgpu.enabled` to true.
- [Safari Technology Preview](https://developer.apple.com/safari/technology-preview/): Enable the Develop menu by going to `Safari` &rightarrow; `Preferences` &rightarrow; `Advanced` &rightarrow; `Show Develop menu in menu bar`. Then go to the `Develop` menu and enable `Experimental Features` &rightarrow; `WebGPU`.

## Articles

- [WebGPU - Wikipedia](https://en.wikipedia.org/wiki/WebGPU)
- [Access modern GPU features with WebGPU](https://web.dev/gpu/) - web.dev (by [François Beaufort](https://github.com/beaufortfrancois) & [Corentin Wallez](https://github.com/Kangz))
- [A Taste of WebGPU in Firefox](https://hacks.mozilla.org/2020/04/experimental-webgpu-in-firefox/) - mozilla.org (by [Dzmitry Malyshau](https://github.com/kvark))
- [Point of WebGPU native](https://kvark.github.io/web/gpu/native/2020/05/03/point-of-webgpu-native) - by [Dzmitry Malyshau](https://github.com/kvark)
- [Graphics on the web and beyond with WebGPU](https://dmnsgn.medium.com/13c4ba049039) - medium.com (by [Damien Seguin](https://dmnsgn.medium.com/))
- [Implementing WebGPU in Gecko](https://kvark.github.io/web/gpu/gecko/2019/12/10/gecko-webgpu) - by [Dzmitry Malyshau](https://github.com/kvark)
- [From WebGL to WebGPU in Construct](https://www.construct.net/en/blogs/ashleys-blog-2/webgl-webgpu-construct-1519) - construct.net (by [Ashley Gullen](https://twitter.com/AshleyGullen))
- [A brief history of graphics on the web and WebGPU](https://www.construct.net/en/blogs/ashleys-blog-2/brief-history-graphics-web-1517) - construct.net (by [Ashley Gullen](https://twitter.com/AshleyGullen))
- [WebGPU texture best practices](https://toji.github.io/webgpu-best-practices/img-textures.html) - by [Brandon Jones](https://github.com/toji)
- [WebGPU Buffer upload best practices](https://toji.github.io/webgpu-best-practices/buffer-uploads.html) - by [Brandon Jones](https://github.com/toji)
- [wgpu-rs on the web](https://gfx-rs.github.io/2020/04/21/wgpu-web) - Rust Graphics Mages
- [Compiling Machine Learning to WASM and WebGPU with Apache TVM](https://tvm.apache.org/2020/05/14/compiling-machine-learning-to-webassembly-and-webgpu) - tvm.apache.org (by [Tianqi Chen](https://github.com/tqchen) & [Jared Roesch](https://github.com/jroesch))
- [The WebAssembly App Gap](https://paulbutler.org/2020/the-webassembly-app-gap/) - by [Paul Butler](https://github.com/paulgb)
- [Next-generation 3D Graphics on the web](https://webkit.org/blog/7380/next-generation-3d-graphics-on-the-web/) - webkit.org (by [Dean Jackson](https://twitter.com/grorgwork))
- [Efficently rendering glTF models - A WebGPU Case Study](https://toji.github.io/webgpu-gltf-case-study/) - by [Brandon Jones](https://github.com/toji)

## Tutorials

- [Raw WebGPU](https://alain.xyz/blog/raw-webgpu) - by [Alain Galvan](https://github.com/alaingalvan)
- [Basic WebGPU Rendering](https://dev.to/ndesmic/basic-webgpu-rendering-2kob) - by [@ndesmic](https://github.com/ndesmic)
- [Get started with GPU Compute on the Web](https://web.dev/gpu-compute/) - web.dev (by [François Beaufort](https://github.com/beaufortfrancois))
- [WebGPU for Metal Developers Part 1](https://metalbyexample.com/webgpu-part-one/) ([Part 2](https://metalbyexample.com/webgpu-part-two/)) - by [Warren Moore](https://twitter.com/warrenm)
- [From 0 to glTF with WebGPU: The First Triangle](https://www.willusher.io/graphics/2021/08/29/0-to-gltf-triangle) (updated version of [this](https://www.willusher.io/graphics/2020/06/15/0-to-gltf-triangle)) - by [Will Usher](https://github.com/Twinklebear)
- [From 0 to glTF with WebGPU: Bind Groups](https://www.willusher.io/graphics/2021/08/30/0-to-gltf-bind-groups) (updated version of [this](https://www.willusher.io/graphics/2020/06/20/0-to-gltf-bind-groups)) - by [Will Usher](https://github.com/Twinklebear)
- [Learn Wpgpu](https://sotrh.github.io/learn-wgpu/): Examples and Showcase Rust & Wgpu - by [@sotrh](https://github.com/sotrh)
- [LearningWebGPU 教程 (Chinese)](https://github.com/hjlld/LearningWebGPU) - by [@hjlld](https://github.com/hjlld)
- [Real-Time Ray-Tracing in WebGPU](https://maierfelix.github.io/2020-01-13-webgpu-ray-tracing/) - by [Felix Maier](https://github.com/maierfelix)
- [Build a compute rasterizer in WebGPU](https://github.com/OmarShehata/webgpu-compute-rasterizer/blob/main/how-to-build-a-compute-rasterizer.md) - by [Omar Shehata](https://github.com/OmarShehata)
- [[Not finished] WebGPU training](https://github.com/drawmindmap/webgpu-training) - by [@DrawMindmap](https://github.com/drawmindmap)
- [WebGPU Engine Development (Chinese/English)](https://arche.graphics/docs/intro): Development process of WebGPU Engine(C++ and TypeScript)
- [Learn WebGPU for native C++ development](https://eliemichel.github.io/LearnWebGPU) - by [@eliemichel](https://github.com/eliemichel)

## Books

- [Practical WebGPU Graphics](https://books.google.com/books?id=tPQyEAAAQBAJ&printsec=frontcover) - by [Jack Xu](https://github.com/jack1232)

## Libraries

- [Babylon.js](https://doc.babylonjs.com/advanced_topics/webGPU) - Experimental support
- [Three.js](https://github.com/takahirox/THREE.WebGPURenderer) - Experimental support
- [Dawn](https://dawn.googlesource.com/dawn) - Google implementation
- [Gfx-rs/wgpu](https://github.com/gfx-rs/wgpu) - Mozilla implementation
- [Webcore module WebGPU](https://trac.webkit.org/browser/webkit/trunk/Source/WebCore/Modules/webgpu) - Webkit / Safari
- [bgfx](https://github.com/bkaradzic/bgfx#bgfx---cross-platform-rendering-library) - WebGPU/Dawn experimental
- [webgpu-headers](https://github.com/webgpu-native/webgpu-headers) - C/C++ headers
- [sokol](https://github.com/floooh/sokol/issues/278) - WebGPU Backend TODO
- [WebGPU for Node](https://github.com/maierfelix/webgpu) - Based on Dawn
- [RedGPU](https://github.com/redcamel/RedGPU) - By @redcamel
- [WebGPU .NET](https://github.com/WaveEngine/WebGPU.NET)
- [Deno roadmap](https://twitter.com/trivikram/status/1275469111674322945) - GPU APIs (WebGPU) to support ML apps
- [RedCube](https://github.com/Reon90/redcube) - GLTF implementation based on WebGPU backend
- [hwoa-rang-gpu](https://github.com/gnikoloff/hwoa-rang-gpu) - micro WebGPU rendering & compute library
- [wgsl_reflect](https://github.com/brendan-duncan/wgsl_reflect) - A WebGPU Shading Language parser and reflection library for Javascript.
- [Arche Graphics](https://github.com/ArcheGraphics) - WebGPU Graphics Engine
- [WebGPU-C++](https://github.com/eliemichel/WebGPU-Cpp) - A single-file zero-overhead C++ idiomatic wrapper - by [@eliemichel](https://github.com/eliemichel)
- [Use.GPU](https://usegpu.live) - Reactive/declarative WebGPU runtime
- [GEngine](https://github.com/hpugis/GEngine) -A basic rendering engine based on WebGPU -by junwei.gu
- [Thimbleberry](https://github.com/mighdoll/thimbleberry) - Reusuable WebGPU shaders and support functions

## Gists

- [3D SDF Primitives](https://gist.github.com/munrocket/f247155fc22ecb8edf974d905c677de1) - in WGSL by @munrocket
- [2D SDF Primitives](https://gist.github.com/munrocket/30e645d584b5300ee69295e54674b3e4) - in WGSL by @munrocket

## Demos

Demos might work only on Chrome. Firefox implementation is not complete.

- [WebGPU Samples](https://austineng.github.io/webgpu-samples/) - by [Austin Eng](https://github.com/austinEng) (Google) - [repository](https://github.com/austinEng/webgpu-samples)
- [WebGPUniverse](https://webgpuniverse.netlify.app) - by students from Imperial College London
- [WebGPU first-person exploration of the Sponza Palace](https://toji.github.io/webgpu-test/) - by [Brandon Jones](https://github.com/toji) - [repository](https://github.com/toji/webgpu-test)
- [WebGPU Clustered Shading](https://toji.github.io/webgpu-clustered-shading/) - by [Brandon Jones](https://github.com/toji) - [repository](https://github.com/toji/webgpu-clustered-shading)
- [WebGPU Metaballs](https://toji.github.io/webgpu-metaballs/) - by [Brandon Jones](https://github.com/toji) - [repository](https://github.com/toji/webgpu-metaballs)
- [WebGPU External Texture Test](https://toji.github.io/webgpu-external-test/) - by [Brandon Jones](https://github.com/toji) - [repository](https://github.com/toji/webgpu-external-test)
- [Online WGSK Editor](https://takahirox.github.io/online-wgsl-editor/) - by [Takahiro](https://github.com/takahirox) - [repository](https://github.com/takahirox/online-wgsl-editor)
- [Safari WebKit demos](https://webkit.org/demos/webgpu/)
- [Three.js WebGPU examples](https://threejs.org/examples/?q=webgpu) - by [Three.js](https://threejs.org) - [repository](https://github.com/mrdoob/three.js/tree/dev/examples#:~:text=webgpu_compute.html)
- [Spookyball: a WebGPU-powered, Halloween-themed game](https://spookyball.com) - by [Brandon Jones](https://github.com/toji) - [repository](https://github.com/toji/spookyball)
- [Babylon.js Playground](https://playground.babylonjs.com/) - by [Babylon.js](https://www.babylonjs.com) (Note: Select `WebGPU` in the top right corner) - [repository](https://github.com/BabylonJS/Babylon.js/tree/master/Playground)
- [Calculate and render particles with WebGPU](https://hsimpson.github.io/webgpu-particles/) - by [Daniel Toplak](https://github.com/hsimpson) - [repository](https://github.com/hsimpson/webgpu-particles)
- [An online WebGPU calculator](https://laskin.live): Using WebGPU on remote browser (via WebRTC) - [repository](https://github.com/periferia-labs/laskin.live)
- [WebGPU study](https://redcamel.github.io/webgpu/) - by [Redcamel](https://github.com/redcamel) - [repository](https://github.com/redcamel/webgpu)
- [Small examples of SPIR-V compatible WebGPU usage](https://tsherif.github.io/webgpu-examples/) - by [Tarek Sherif](https://github.com/tsherif) - [repository](https://github.com/tsherif/webgpu-examples)
- [WebGPU examples](https://wgpu.rs/examples-gpu/) - by [wgpu.rs](https://wgpu.rs) - [repository](https://github.com/gfx-rs/wgpu/tree/master/wgpu/examples)
- [Three.js WebGPURenderer](https://takahirox.github.io/THREE.WebGPURenderer/examples/) - by [Takahiro](https://github.com/takahirox) - [repository](https://github.com/takahirox/THREE.WebGPURenderer)
- [WebGPU point cloud](https://m-schuetz.github.io/webgpu_pointcloud/) - by [Markus Schütz](https://github.com/m-schuetz) - [repository](https://github.com/m-schuetz/webgpu_pointcloud)
- [Forest WebGPU](https://www.babylonjs.com/demos/webgpu/forestwebgpu) - by [Babylon.js](https://www.babylonjs.com)
- [WebGPU-Playground](https://06wj.github.io/WebGPU-Playground/) - by [@06wj](https://github.com/06wj) - [repository](https://github.com/06wj/WebGPU-Playground)
- [node-webgpu examples](https://github.com/maierfelix/webgpu-examples) - by [Felix Maier](https://github.com/maierfelix)
- [Dawn RT (Ray tracing extension for Dawn/WebGPU)](https://github.com/maierfelix/dawn-ray-tracing) - by [Felix Maier](https://github.com/maierfelix)
- [WebGPU Experiments](https://www.willusher.io/webgpu-experiments/) - by [Will Usher](https://github.com/Twinklebear) - [repository](https://github.com/Twinklebear/webgpu-experiments)
- [wgpu-load-test](https://github.com/MacTuitui/wgpu-load-test) - by [Alexis Andre](https://github.com/MacTuitui)
- [WGSL-Toy](https://valeerajs.github.io/WGSL-Toy/build/) - by [@HypnosNova](https://github.com/HypnosNova) - [repository](https://github.com/ValeeraJS/WGSL-Toy)
- [WebGPU Compute 101 Demo](https://hello-webgpu-compute.glitch.me) - [source code](https://glitch.com/edit/#!/hello-webgpu-compute)
- [WebGPU: Rendering, compute, GPU experiments](https://oktomus.com/web-experiments/) - by [Kevin Masson](https://github.com/oktomus) - [repository](https://github.com/oktomus/web-experiments)
- [WebGPU Sketch Dojo](https://gnikoloff.github.io/webgpu-dojo/) - by [Georgi Nikolov](https://github.com/gnikoloff) - [repository](https://github.com/gnikoloff/webgpu-dojo)
- [WebGPU Compute Metaballs](https://gnikoloff.github.io/webgpu-compute-metaballs/) - by [Georgi Nikolov](https://github.com/gnikoloff) - [repository](https://github.com/gnikoloff/webgpu-compute-metaballs)
- [WebGPU 2D Fluid Simulation](https://github.com/indiana-dev/WebGPU-Fluid-Simulation) - by [indiana-dev](https://github.com/indiana-dev) - [repository](https://github.com/indiana-dev/WebGPU-Fluid-Simulation)
- [WebGPU-Lab](https://s-macke.github.io/WebGPU-Lab/) - by [Sebastian Macke](https://github.com/s-macke) - [repository](https://github.com/s-macke/WebGPU-Lab)
- [WebGPU Live Demo Editor](https://www.wgsl.dev/editor) - by [Hepp Maccoy](https://github.com/hepp) - [repository](https://github.com/hepp/webgpu-examples)
- [Thimbleberry Image Transform Demo](https://thimbleberry.dev) - by [mighdoll](https://vis.social/@mighdoll) - [repository](https://github.com/mighdoll/thimbleberry/tree/main/image-demo)

## Videos

- [From WebGL to WebGPU: A perspective from Babylon js by David Catuhe](https://www.youtube.com/watch?v=A2FxeEl4nWw)
- [Next-Generation 3D Graphics on the Web (Google I/O ’19)](https://www.youtube.com/watch?v=K2JzIUIHIhc)
- [WebGPU (playlist)](https://www.youtube.com/playlist?list=PLMinhigDWz6f5Nm_GYGREYnaf9mzoNdjX) - by [SketchpunkLabs](https://www.youtube.com/c/SketchpunkLabs)
- [WebGPU (playlist)](https://www.youtube.com/playlist?list=PLnTPVrg9-a1Ou2KXUniDr1HC7qgL2JD2x) - by [Genka](https://www.youtube.com/channel/UCBTwKzJg-BR56tKWO5CT7XA)
- [WebGPU Graphics Programming Step-by-Step (playlist)](https://www.youtube.com/playlist?list=PL_UrKDEhALdKh0118flOjuAnVIGKFUJXN) - by [Practical Programming with Dr. Xu](https://www.youtube.com/channel/UCg14XfqXim0vpgabU3T7tRg)

## Presentations

- [Tint](https://docs.google.com/presentation/d/1qHhFq0GJtY_59rNjpiHU--JW4bW4Ji3zWei-gM6cabs) - Proposal for textual shader language by Google
- [Building WebGPU with Rust](https://fosdem.org/2020/schedule/event/rust_webgpu/) - by [Dzmitry Malyshau](https://github.com/kvark) from Mozilla

## Community

- [GPU for the web community group](https://www.w3.org/community/gpu/) - W3C Community
- [Public GPU](https://lists.w3.org/Archives/Public/public-gpu/) - W3C Mailing list
- [Gitter chat](https://gitter.im/gfx-rs/webgpu) - by Mozilla - DEPRECATED
- [Matrix WebGPU](https://matrix.to/#/#WebGPU:matrix.org) - Unofficial channel
- [YC Point of WebGPU on native](https://news.ycombinator.com/item?id=23079200) - discussion regarding this article
- [Possibility of SPIR-V and/or GLSL as a WebGPU extension?](https://github.com/gpuweb/gpuweb/issues/847) - WGSL in debate

## Bug reporting

- [Webkit](https://bugs.webkit.org/buglist.cgi?bug_status=UNCONFIRMED&bug_status=NEW&bug_status=ASSIGNED&bug_status=REOPENED&component=WebGPU)
- [Firefox](https://bugzilla.mozilla.org/buglist.cgi?product=Core&component=Graphics%3A%20WebGPU)
- [Chromium](https://bugs.chromium.org/p/chromium/issues/list?q=component:Blink%3EWebGPU)

## Contribute

Contributions welcome! Read the [contribution guidelines](contributing.md) first.

## License

[![CC0](https://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](https://creativecommons.org/publicdomain/zero/1.0)

To the extent possible under law, Mik BRY has waived all copyright and
related or neighboring rights to this work.
