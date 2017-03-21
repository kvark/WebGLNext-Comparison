# Unofficial comparison of WebGL-Next API proposals

APIs                      | WebGPU-Apple | NXT-Google  | Obsidian-Mozilla
------------------------- | ------------ | ----------- | ---------------------
**General:**              |              |             |
based on                  | [Metal](https://developer.apple.com/metal/) | -/- | [Vulkan](https://www.khronos.org/vulkan/)
officially proposed       | [yes](https://github.com/gpuweb/proposals/blob/master/WebGPU-Apple/api-proposal.html) | not yet | [yes](https://github.com/KhronosGroup/WebGLNext-Proposals/tree/master/Obsidian-Mozilla)
prototype implementation  | [Webkit](https://bugs.webkit.org/show_bug.cgi?id=167952) | [Chromium](https://github.com/gpuweb/nxt-chromium) | none yet
shader format             | some IR      | SPIR-V (currently) | SPIR-V
target platforms          | web          | web (asm first), native | web (asm first)
**Features:**             |              |             |
command buffers           | X            | X           | X
secondary command buffers |              | TBD         | [experimental](https://github.com/KhronosGroup/WebGLNext-Proposals/tree/master/Obsidian-Mozilla#secondary-command-buffers)
pipeline state objects    | X            | X           | X
compute pipelines         | X            | X           | X
tessellation              |              |             |
descriptor sets           |              | X           | X
render sub-passes         |              | TBD         | X
transient resources       |              | TBD         | X
resource layouts          |              | X           | X
