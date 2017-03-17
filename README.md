# Unofficial comparison of WebGL-Next API proposals

APIs                      | WebGPU-Apple | NXT-Google  | Obsidian-Mozilla
------------------------- | ------------ | ----------- | ---------------------
**General:**              |              |             |
based on                  | [Metal](https://developer.apple.com/metal/) | -/- | [Vulkan](https://www.khronos.org/vulkan/)
officially proposed       | [yes](https://github.com/gpuweb/proposals/blob/master/WebGPU-Apple/api-proposal.html) | not yet | [yes](https://github.com/KhronosGroup/WebGLNext-Proposals/pull/2)
prototype implementation  | [Webkit](https://bugs.webkit.org/show_bug.cgi?id=167952) | [Chromium](https://github.com/gpuweb/nxt-chromium) | none yet
shader format             | some IR      | SPIR-V      | SPIR-V
target platforms          | web          | native, web | web (assembly first)
target audience           | people       | people      | engines/frameworks
**Features:**             |              |             |
command buffers           | X            | X           | X
secondary command buffers |              |             | [experimental](https://github.com/kvark/WebGLNext-Proposals/blob/obsidian/Obsidian-Mozilla/README.md#secondary-command-buffers)
pipeline state objects    | X            | X           | X
compute pipelines         | X            | X           | X
tessellation              |              |             |
descriptor sets           |              | X           | X
render sub-passes         |              |             | X
transient resources       |              |             | X
