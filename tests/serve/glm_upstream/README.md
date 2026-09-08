# Vendored GLM chat template

`chat_template.jinja` in this directory is a byte-for-byte copy of the chat
template shipped with the upstream GLM-5.3-Flash release. It exists so the
tool-protocol oracle in `tests/serve/test_glm_upstream.py` — and the CI job
that runs it — never depends on a model download or a machine-local
`~/models` checkout.

- Source:
  <https://huggingface.co/zai-org/GLM-5.3-Flash/resolve/eb9eb208eb0d988989d07a6a12d0fdeb5f52574a/chat_template.jinja>
  (the sibling code repository, <https://github.com/zai-org/GLM-5>, is
  Apache-2.0 but does not ship the template; the template lives in the
  Hugging Face model repository)
- Upstream revision: `eb9eb208eb0d988989d07a6a12d0fdeb5f52574a`
- SHA-256 of the vendored file:
  `0c4099f3382d6c92700dfb99725025360966fd73032f0ecf32377c0d9e6309c5`
- License: MIT. The Hugging Face model repository is tagged `license:mit`.
  The template is redistributed here under that MIT license; the upstream
  LICENSE is at
  <https://huggingface.co/zai-org/GLM-5.3-Flash/blob/eb9eb208eb0d988989d07a6a12d0fdeb5f52574a/LICENSE>.

Copyright (c) Z.ai / zai-org

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

Used in CI oracle tests with FakeEngine; no real GLM model or weights are
used.
