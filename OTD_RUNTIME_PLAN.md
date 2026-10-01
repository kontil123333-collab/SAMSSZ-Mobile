# OTD runtime plan

The supplied SamsszConverter.py already embeds the exact RageBuilder payload and extracts it at Python import time. This Android port preserves that engine. The missing Android-specific layer is the ARM64 runtime which can execute the embedded Windows x86-64 `ragebuilder.exe`.

The port therefore supports a complete runtime pack under `otd_runtime/` and stages `HOME` there while invoking the original OTD engine. No fake/native replacement builder is used.

The runtime stack follows the same class of approach documented by Box64/Wine: Box64 translates x86-64 Linux-side components on ARM64 and Wine provides the Windows API compatibility layer. XoW64 packages Wine-WoW64 + Box64 for aarch64 Termux/proot environments.
