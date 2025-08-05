# UnrealGitPluginTest
This is a test repo to demonstrate a bug in Unreal Engine Git Plugin

To Reporoduce the issue:

1. Clone the repository
2. Set active branch to `Branch_B`
3. Merge `main` into `Branch_B`

*the conflict will emerge, do not resolve it

4. Open Unreal Editor
5. Link to Git (using settings in the lower right corner)
6. Right Click the `BP_TestActor` -> `Revision Control` -> `Merge`
<img width="835" height="1060" alt="image" src="https://github.com/user-attachments/assets/a8ad9ea8-b764-4886-aa1e-3a2e5dca019b" />


* you will notice that merging commit is not the latest 
<img width="862" height="709" alt="image" src="https://github.com/user-attachments/assets/0a0f6937-752a-4022-9483-f0237745bd2e" />


7. You can click `Start Merge` to confirm the issue

Expected:
On merge the latest `a5dff52` commit should be visible in Unreal Editor


<img width="407" height="127" alt="image" src="https://github.com/user-attachments/assets/ca565561-468b-485c-a65b-cfcdd76fdae3" />
