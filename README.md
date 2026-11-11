# bgfx workspace

三个上游仓库并列放在同一工作区，bgfx 的构建脚本要求这种布局：

- `bgfx/`  主工程
- `bx/`    基础库（提供 genie 构建工具）
- `bimg/`  图像/纹理工具链依赖

构建（Linux）：

```bash
cd bgfx
make linux-gcc-release64 -j$(nproc)
# 产物在 bgfx/.build/linux64_gcc/bin/
```

上游对应提交：
- bgfx  f5ce45e39d6381093e577e80adb1abb2c611302c
- bx    57548da89a07771c5b0f8a6711149be70e08a329
- bimg  77bebb28e12956bfced82bb2cf7c19ac5735b6c8
