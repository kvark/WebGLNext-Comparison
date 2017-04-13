# Unofficial comparison of WebGL-Next API proposals

APIs                      | WebGPU       | NXT         | Obsidian
------------------------- | ------------ | ----------- | ---------------------
**General:**              |              |             |
author                    | Apple        | Google      | Mozilla
based on                  | [Metal](https://developer.apple.com/metal/) | -/- | [Vulkan](https://www.khronos.org/vulkan/)
officially proposed       | [yes](https://github.com/gpuweb/proposals/blob/master/WebGPU-Apple/api-proposal.html) | not yet | [yes](https://github.com/KhronosGroup/WebGLNext-Proposals/tree/master/Obsidian-Mozilla)
prototype implementation  | [Webkit](https://bugs.webkit.org/show_bug.cgi?id=167952) | [Chromium](https://github.com/gpuweb/nxt-chromium) | none yet
shader format             | some IR      | SPIR-V (currently) | SPIR-V
target platforms          | JS, WASM?    | WASM, JS, native | WASM, JS
run-time validation       | always       | always      | optional
**Features:**             |              |             |
command buffers           | +            | +           | +
secondary command buffers | -            | ?           | [experimental](https://github.com/KhronosGroup/WebGLNext-Proposals/tree/master/Obsidian-Mozilla#secondary-command-buffers)
multiple command queues   | +            | ?           | +
pipeline state objects    | +            | +           | +
compute pipelines         | +            | +           | +
descriptor sets           | -            | +           | +
render sub-passes         | -            | ?           | +
transient resources       | -            | ?           | +
resource layouts          | -            | +           | +
