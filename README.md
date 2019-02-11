# RhythmJump
A music based platform game

## Docs

- Chinese GDD: [Google Docs](https://docs.google.com/document/d/1o8JgMRD53AjWpdXvaA8AGeciMkFDwY28pzybJHmWqKY/edit)
- English GDD: [Google Docs](https://docs.google.com/document/d/1kXH58Myj2T4DLfro5Uc1xLvNs8SQxa3L3cDC9CGhSiI/edit)

## Development

Reference:

- Basic Git operations: [The Tutorial](https://git-scm.com/docs/gittutorial) (Only basics are required)

- Use Git with UE4 projects: [Unreal Wiki](https://wiki.unrealengine.com/Git_source_control_(Tutorial)) (Important steps are described below)

### Get Started

1. Clone the repo.

2. Use [Git LFS](https://git-lfs.github.com/) to track binary file.

   1.  Install Git LFS ([Guide](https://help.github.com/articles/installing-git-large-file-storage)).

   2. Track binary file types with Git LFS (extend it if more binary types are introduced, e.g. mp3/jpg/png):

      ```shell
      git lfs install
      git lfs track "*.uasset"
      git lfs track "*.umap"
      git lfs track "*.wav"
      ```

3. You may now perform normal git operations on this repo.

### Configure Unreal Engine Editor (Optional)

1. Open the UE4 project `RhythmJump.uproject`.
2. Open `Source Control` in toolbar and select `Change Source Control Settings ...`.
3. In the pop-up window, switch the provider to `Git (beta version)` and confirm the path of git executable is correctly filled in `Git Path` .
4. Select `Accept Settings` and its done.
5. You can now add/submit(commit) files in UE4 Editor. 

### Notes

- Default `.gitignore` file is used, provided by GitHub. Modify it if needed.
- You may still need to use the command line tools or Git GUI to perform the push/pull/branch/merge operations since I didn't find it in the editor plugin.
- Whatever method you are using, remember to perform `git pull`  before start working to avoid merge conflicts. Also, try to communicate with the team when you are going to make a change,  pull/commit/push frequently and make everyone happy.

## Contributors

- Peifeng Ye

- Dinghan Zhu

- Qiming Du
- Juanrui Zhao
- Chuanzhe Li