# ArcDesktop

The default DE (+ WM) for Neutron.

ArcDE by default allows stacked windows with z-indices like the CSS box model. The key is to allow windows to be dragged around and truncated across the edge. And be resized according to the app's spec.

## Dioxus

Dioxus is prob the greatest thing Ive seen up to now. Rust with react semantics. We have our own icons and material/bootstrap icons (transparent).

I dont think it has a live debug build/hot reload capability. Since we would need a rust interpreter or JIT. But its pretty good.

## Apps

Apps must be runnable on ArcWM. I.e. it should have code that uses the ArcWM API to create a window and render its stuff within it. Its rendering engine can either use NeutronDRM or indirectly use it through Dioxus desktop (wgpu, which then uses NeutronDRM).
