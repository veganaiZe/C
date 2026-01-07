OpenGL
======

  - _References_
    | Version                                                                       | Format | Notes
    |-------------------------------------------------------------------------------|--------|------
    | [OpenGL 2.1 Reference](https://registry.khronos.org/OpenGL-Refpages/gl2.1/)   | HTML   | Includes GLX & GLU
    | [OpenGL 3.2 Reference](https://registry.khronos.org/OpenGL-Refpages/es3/)     | HTML   | Last Apple (stock)
    | [OpenGL 3.2 QuickRef](https://www.khronos.org/files/opengl-quick-reference-card.pdf)   | PDF | Last Apple (stock)
    | [OpenGL 4.1 QuickRef](https://www.khronos.org/files/opengl41-quick-reference-card.pdf) | PDF | Last Apple (upgrade)
    | [OpenGL 4.5 Reference](https://registry.khronos.org/OpenGL-Refpages/gl4/bottom.php) | HTML   |
    | [OpenGL 4.6 (core) QuickRef](https://www.khronos.org/files/opengl46-quick-reference-card.pdf) | PDF |
    | [glTF 2.0 QuickRef](https://www.khronos.org/files/gltf20-reference-guide.pdf) | PDF    |
  - [_Specifications_](https://registry.khronos.org/OpenGL/specs/gl/)
    | Version                                                                             | Format | Notes
    |-------------------------------------------------------------------------------------|--------|------
    | [OpenGL 2.1](https://registry.khronos.org/OpenGL/specs/gl/glspec21.pdf)             | PDF    |
    | [OpenGL 3.3 (core)](https://registry.khronos.org/OpenGL/specs/gl/glspec33.core.pdf) | PDF    |
    | [OpenGL 4.1 (core)](https://registry.khronos.org/OpenGL/specs/gl/glspec41.core.pdf) | PDF    | ES 2.0 Compatible, Last Apple Version
    | [OpenGL 4.6 (core)](https://registry.khronos.org/OpenGL/specs/gl/glspec46.core.pdf) | PDF    |
    | [Extensions](https://registry.khronos.org/OpenGL/extensions/)                       | TXT    |
  - _Libraries_
    - [GLEW](https://github.com/nigels-com/glew) - extension wrangler
      - [usage](https://glew.sourceforge.net/basic.html) - initializing & checking for extensions
    - [GLM](https://github.com/g-truc/glm) - mathematics
    - [GLU 1.3](https://registry.khronos.org/OpenGL/specs/gl/glu1.3.pdf) - utility (pdf)
    - [GLUS](https://github.com/McNopper/GLUS) - cross graphic library utilities
    - [GLUT](https://en.wikipedia.org/wiki/OpenGL_Utility_Toolkit) - utility toolkit (gui)
      - [GLUT API](https://www.opengl.org/resources/libraries/glut/spec3/spec3.html) ( [pdf](https://www.opengl.org/resources/libraries/glut/glut-3.spec.pdf) )
      - [freeglut API](https://freeglut.sourceforge.net/docs/api.php)
        - [glut-compatible api](https://raw.githubusercontent.com/freeglut/freeglut/refs/heads/master/include/GL/freeglut_std.h)
        - [non-glut-compatible extensions api](https://raw.githubusercontent.com/freeglut/freeglut/refs/heads/master/include/GL/freeglut_ext.h)
        - [callbacks with user data arguments](https://raw.githubusercontent.com/freeglut/freeglut/refs/heads/master/include/GL/freeglut_ucall.h)
    - [GLX 1.4](https://registry.khronos.org/OpenGL/specs/gl/glx1.4.pdf) - x11 interface to opengl (pdf)
    - [WGL](https://learn.microsoft.com/en-us/windows/win32/api/_opengl/) - win32 interface to opengl
    - [Mesa 3D](https://mesa3d.org/) - open source implementation w/ software fallback
      - [EGL](https://registry.khronos.org/EGL/) - interface window system to rendering api
        - [Reference](https://registry.khronos.org/EGL/sdk/docs/man/) - 1.5 (html)
        - [Quick Ref](https://www.khronos.org/files/egl-1-4-quick-reference-card.pdf) - 1.4 (pdf)
  - _Knowledge_
    - Mathematics
      - [Math2.org](http://math2.org/)
      - [3D Geometry Primer]() - flipcode
      - [Immersive Linear Algebra](https://immersivemath.com/ila/index.html)
    - Books
      - [Learning Modern 3D Graphics Programming](https://www.cse.chalmers.se/edu/year/2018/course/TDA361/LearningModern3DGraphicsProgramming.pdf) - pdf
      - OpenGL SuperBible
        - 5th edition
          - [code, files, libraries](https://web.archive.org/web/20130124081158id_/http://www.starstonesoftware.com/files/SB5.zip)
          - [source archive](https://web.archive.org/web/20170102030551id_/https://storage.googleapis.com/google-code-archive-source/v2/code.google.com/oglsuperbible5/source-archive.zip) - google code
          - [mac xcode](https://web.archive.org/web/20130417020646id_/http://www.starstonesoftware.com/files/XCode.zip) - back ported to opengl 2.1 for [old macs](http://web.archive.org/web/20110110182311id_/http://www.starstonesoftware.com/OpenGL/mac.htm)
        - 6th edition
          - [source code](https://web.archive.org/web/20140209130615id_/http://openglsuperbible.com/files/sb6code_2013_11_10.zip) ( [github](https://github.com/openglsuperbible/sb6code) )
          - [media archive](https://web.archive.org/web/20140209130615id_/http://openglsuperbible.com/files/sb6media_2013_11_10.zip)
        - 7th edition
          - [source code](https://github.com/openglsuperbible/sb7code/archive/master.zip) ( [github](https://github.com/openglsuperbible/sb7code) )
          - [media archive](https://web.archive.org/web/20170929211831id_/http://openglsuperbible.com/files/superbible7-media.zip)
      - Realtime Rendering
        - [Collision Detection](http://web.archive.org/web/20241212124841id_/https://www.realtimerendering.com/Real-Time_Rendering_4th-Collision_Detection.pdf) - pdf
        - [Real-Time Ray Tracing](http://web.archive.org/web/20241212124841id_/https://www.realtimerendering.com/Real-Time_Rendering_4th-Real-Time_Ray_Tracing.pdf) - pdf
        - [Appendicies](http://web.archive.org/web/20241212124841id_/https://www.realtimerendering.com/Real-Time_Rendering_4th-Appendices.pdf) - pdf, linear algebra & trig
      - The Red Book
        - [online html](https://web.archive.org/web/20131009113357id_/https://fly.cc.fer.hr/~unreal/theredbook/)
        - [code samples](https://www.opengl.org/archives/resources/code/samples/redbook/)
        - [pdf](https://w2.mat.ucsb.edu/594cm/2009/docs/RedBook.pdf)
        - [zipped html book](https://web.archive.org/web/20130430205318id_/http://fly.cc.fer.hr/~unreal/theredbook/theredbook.zip)
        - Code Samples - 5th ed ( [opengl 1.0](http://web.archive.org/web/20070216025655id_/http://www.opengl-redbook.com/source/OpenGL-1.0.zip) ) ( [opengl 1.1](http://web.archive.org/web/20070216025655id_/http://www.opengl-redbook.com/source/OpenGL-1.1.zip) ) ( [opengl 1.2](http://web.archive.org/web/20070216025655id_/http://www.opengl-redbook.com/source/OpenGL-1.2.zip) ) ( [opengl 1.4](http://web.archive.org/web/20070216025655id_/http://www.opengl-redbook.com/source/OpenGL-1.4.zip) )
        - Code Samples - 8th ed ( [opengl 4.3](http://web.archive.org/web/20160316053103id_/http://www.opengl-redbook.com/Code/oglpg-8th-edition.zip) )
        - Code Samples - 9th ed ( [opengl 4.5](http://opengl-redbook.com/OGLPG-9th-Edition.zip) ) ( [_github_](https://github.com/openglredbook/examples) )
        - [`gl3.h`](https://raw.githubusercontent.com/openglredbook/examples/refs/heads/master/include/GL3/gl3.h)
    - Wikis
      - [OpenGL wiki](https://www.khronos.org/opengl/wiki/Main_Page) - khronos
        - [History of OpenGL](https://wikis.khronos.org/opengl/History_of_OpenGL)
        - [History of Programmability](https://wikis.khronos.org/opengl/History_of_Programmability)
        - [Tutorials](https://wikis.khronos.org/opengl/Tutorials)
      - [OpenGL](https://en.wikipedia.org/wiki/OpenGL) - wikipedia
    - Slides
      - [Math Cheatsheet](http://www.opengl-tutorial.org/miscellaneous/math-cheatsheet/)
      - [3d Maths Cheat Sheet](https://antongerdelan.net/teaching/3dprog1/maths_cheat_sheet.pdf)
      - [Everything you ever wanted to know about collision detection](https://courses.cs.duke.edu/spring08/cps124/notes/13_collisions/collision_detection.pdf)
    - Tutorials
      - [anton's opengl 4 tutorials](https://antongerdelan.net/opengl/)
      - [learnopengl.com](https://learnopengl.com/)
      - [modern opengl guide](https://open.gl/) - open.gl ( [pdf 2017](http://www.openvisionnetworks.com/dist/Modern%20OpenGL%20Guide.pdf) )
      - [opengl4 tutorials](https://sibras.github.io/OpenGL4-Tutorials/docs/Tutorials/01-Tutorial1/) - opengl 3.x - 4.4 ( [github](https://github.com/sibras/OpenGL4-Tutorials) ) ( [pdf](https://riptutorial.com/Download/opengl.pdf) )
      - [openglbook.com](https://openglbook.com/the-book.html)
      - [opengl step by step](https://ogldev.org/) - ogldev.org
      - [opengl tutorial](https://riptutorial.com/opengl) - riptutorial.com
        - [cross platform opengl context creation using sdl2](https://riptutorial.com/opengl/example/15725/cross-platform-opengl-context-creation--using-sdl2-)
      - [Introduction to Computer Graphics](https://math.hws.edu/eck/cs424/graphicsbook-1.3/index.html) - eck
      - [Fundamental OpenGL Tutorials and Notes](http://www.songho.ca/opengl/index.html) - songho
      - [Graphics Programming](https://www.cprogramming.com/graphics-programming.html) - cprogramming.com
      - [Lazy Foo' Productions](https://lazyfoo.net/tutorials/OpenGL/index.php)
      - [Learning Modern 3D Graphics Programming](https://paroj.github.io/gltut/index.html) ( [_github_](https://github.com/paroj/gltut) )
      - [Lighthouse3d](http://www.lighthouse3d.com/tutorials/) - includes glut & glsl tutorials
      - [NeHe](http://nehe.gamedev.net/) ( [_zipped letter pdf_](https://web.archive.org/web/20100706105235id_/http://nehe.gamedev.net/files/resources/nehe_opengl_letter_book_pdf.zip) )
      - [OpenGL Programming](https://en.wikibooks.org/wiki/OpenGL_Programming) - wikibooks
  - _GLSL_
    - [GLSL 1.05](http://web.archive.org/web/20040611122255id_/http://www.opengl.org/documentation/oglsl/ShaderSpecV1.051.pdf) - PDF, extension to opengl 1.4
    - [GLSL 1.20](https://registry.khronos.org/OpenGL/specs/gl/GLSLangSpec.1.20.pdf) - PDF, coincides with opengl 2.1
    - [GLSL 3.30](https://registry.khronos.org/OpenGL/specs/gl/GLSLangSpec.3.30.pdf) - PDF
    - [GLSL 4.10](https://registry.khronos.org/OpenGL/specs/gl/GLSLangSpec.4.10.pdf) - PDF, last apple version
    - [GLSL 4.60](https://registry.khronos.org/OpenGL/specs/gl/GLSLangSpec.4.60.html) - HTML
    - [GLSL Programming](https://en.wikibooks.org/wiki/GLSL_Programming) - wikibooks
    - [Graphics Shaders](https://www.cs.vu.nl/~eliens/download/literatuur-shaders.pdf) - PDF, vrije universiteit amsterdam
    <!-- [GPUOpen Archive](https://gpuopen.com/archive/) -->
  - _Demos / Samples_
    - [Leo - Sneeze the Day demo](http://web.archive.org/web/20151202141514if_/http://developer.amd.com/wordpress/media/2012/10/AMD-Demo-Leo-v1.1.msi) - amd ( [1080p mov](http://web.archive.org/web/20120514115232if_/http://media.amddevcentral.com/video/gpu_videos/Leo_1080p.mov) )
    - [OpenGL 3 & 4](https://github.com/McNopper/OpenGL) - GLUS / GLFW / GLEW
    - [OpenGL 4 examples](https://github.com/markkilgard/opengl4_examples) 2012, Mark Kilgard
    - [OpenGL for X](https://github.com/markkilgard/opengl_for_x) - 1996, Mark Kilgard
    - [OpenGL Samples Pack](https://github.com/g-truc/ogl-samples)
  - _Tools_
    - [CodeXL](https://github.com/GPUOpen-Archive/CodeXL) - debug / profile / analysis
    - [RenderMonkey](http://web.archive.org/web/20110707130949id_/http://download2-developer.amd.com/amd/GPU/executables/RenderMonkey.2008-12-17-v1.82.322.msi) - shader development environment (opengl 2.0, windows)
      - [Release Notes](http://web.archive.org/web/20120526081437id_/http://developer.amd.com/gpu_assets/rendermonkey-releasenotes-v.1.82.320.txt)
      - [SDK Documentation](http://web.archive.org/web/20120526081345id_/http://developer.amd.com/gpu_assets/SDK%20Documentation.pdf)
      - [COLLADA OpenGL Effects Viewer](http://web.archive.org/web/20110911082316id_/http://download2-developer.amd.com/amd/GPU/zip/osg2.2_collada_gl_fx_viewer_031108.zip)
    - [Shader Editor](https://f-droid.org/packages/de.markusfisch.android.shadereditor/) - create and edit GLSL shaders (android 4.0+)
