This is a pre-built opendl32.dll for 64-bit Windows systems.
It was obtained from <http://mesa.fdossena.com/>

Mesa's License text can be found here:
https://docs.mesa3d.org/license.html
(a mixture of largely MITish licenses)

Only an x64 build is vendored; mesa.fdossena.com does not publish a Windows
arm64 build.  On arm64 `wezterm-gui/build.rs` simply skips it and wezterm uses
the system OpenGL driver instead, so `prefer_swrast` has no bundled fallback
there.
