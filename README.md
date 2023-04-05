# ikvm-community
How to build IKVM


## [WIP] Update 5thApril2023
- Use Develop Branch
       <img src="https://user-images.githubusercontent.com/49812372/230218458-93efeebd-d808-445b-b0c5-7f77b2ac43d9.png" width=200px>
     > Native library was removed and replaced with LLVM generated trampolines. So it needs LLVM. But a plain install of LLVM is fine. No WSL needed
- Add LLVM through Visual Studio Installer (do not need => https://releases.llvm.org/download.html)
- Must use the Visual Studio Developer (Command Prompt|PowerShell) for Path extensions

<details>
<summary><strong>[Abandoned PR]</strong>: Build OpenJDK without docker image</summary>

https://github.com/ikvm-revived/ikvm/pull/289

</details>
<details>
<summary>Previous</summary>


https://github.com/ikvm-revived/ikvm/blob/develop/CONTRIBUTING.md#build

> The GitHub action's generated artifact can simply be extract into the appropriate spot in `openjdk/build` to avoid building it yourself. Navigate to the GitHub Actions, find the latest successfuly build for the branch you're concerned with, and download the `openjdk-build-linux-x86_64-normal-server-release` artifact. Extract this zip file into `openjdk/build`.

</details>
