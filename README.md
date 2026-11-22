# ONNX Runtime — pinned mirror

Linux builds of ONNX Runtime **1.19.2**, mirrored for reproducible Docker builds.

## Why this exists

`github.com/microsoft/onnxruntime` no longer resolves — the repo and all its
release assets return 404, so the published tarball URLs are dead. These
archives are repacked from the still-available NuGet package so builds that
need `libonnxruntime` + the C API headers keep working.

## Provenance

- Source: `nuget.org/packages/Microsoft.ML.OnnxRuntime/1.19.2`
- Upstream commit: `ffceed9d44f2f3efb9dd69fa75fea51163c91d91`
- Repacked to match Microsoft's original tarball layout (`lib/`, `include/`)

## Contents

Each archive holds one platform's shared library, the 9 C/C++ API headers, and
the upstream `LICENSE` + `ThirdPartyNotices.txt`.

| Asset | sha256 |
|---|---|
| `onnxruntime-linux-aarch64-1.19.2.tgz` | `54c55d1a122c7e419c3f86b63d47bfae0ce3aa20ac8f3104fce8b95179cd6f69` |
| `onnxruntime-linux-x64-1.19.2.tgz` | `ab5116d880ffd8b6741180add3254ecee8845eebb255c34259985b9b935476ef` |

## Licence

ONNX Runtime is MIT, © Microsoft Corporation. The licence and third-party
notices are included inside each archive, as MIT requires.
