# ikvm-community
How to build IKVM

## [WIP] Update 10th April 2023

[CONTRIBUTING.md](https://github.com/ikvm-revived/ikvm/blob/develop/CONTRIBUTING.md)

Create a build directory in openjdk
- ikvm\openjdk\build 
  >  instead of building openjdk, which needs WSL, get it from Github Action
  > Artifacts are there: https://github.com/ikvm-revived/ikvm/actions/runs/4536287480
  > Click on a build result for a relevant branch (typically you'll want to use **develop**)  

<img src="https://user-images.githubusercontent.com/49812372/230931536-05db3cf8-dd99-4460-ad45-ad9d1725dd68.png" alt="ikvm" width=800px>


  > Scroll down to the bottom of the list to locate `openjdk-build-linux-x86_64-normal-server-release`. Download this zip file from this link and unzip into `openjdk/build.`

<img src="https://user-images.githubusercontent.com/49812372/230930440-bce40cb0-254f-4a11-998c-f3e1897fd030.png" alt="ikvm" width=400px>


## [WIP] Update 5thApril2023

> Current: [ikvm-jdk8u51-b34](https://github.com/ikvm-revived/jdk8u/tree/ikvm-jdk8u51-b34)

> <strong>Next___</strong>: [ikvm-jdk8u60-b32](https://github.com/ikvm-revived/ikvm/pull/290)


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
