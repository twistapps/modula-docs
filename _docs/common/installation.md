
There are multiple ways to install Modula, we recommend using it as [UPM](https://docs.unity3d.com/Manual/upm-ui.html) Git dependency:
{: .notice--info}
### 1. Unity Package Manager Git Dependency
- In Unity, go to _Window_ ▶ _Package Manager_
- Click **"+"** ▶ _Add Package from Git URL..._
- Paste this line: `https://github.com/twistapps/modula.git`
- Wait for unity to download the package for you!

[![](/assets/img/modula-installation-git.gif)](/assets/img/modula-installation-git.gif)
**Click** on the image to see in full screen
{: .notice}

#### `Pros & Cons`
- **Faster updates**: don't need to wait for Unity team to approve the package.
Download updates right when they're ready and published
- **"Under the Hood"** usage: no code in your `Assets/` folder at all.

con: Not so straightforward to dig into the source code because it's hidden in
`Packages/` folder.

Choose this method if you want Modula to work under the hood without littering your `Assets/` folder.
{: .notice--success}

---

### 2. Download from Asset Store
- Go to **Unity Asset Store** (we are working on publishing the package to Unity Asset Store.
After it's published, the link will be available here.)
- Add the package to your account.
- Click "Download"
- Follow further instructions
#### `Pros`
- **Flexibility**: the source code is explicit and possesses its own `Twistapps/Modula` folder.

Choose this method if you want to experiment with Modula's sources yourself.
{: .notice--success}

### 3. Manual Installation
We **do not** recommend this method because it's harder to get updates when Modula is installed manually.
{: .notice--warning}
## Updating
Don't forget to check for updates from time to time! Periodically we provide some new features
and bugfixes
- In Unity, go to _Window_ ▶ _Package Manager_
- Choose **"Packages: In Project"** at the top of the UPM window.
- Find "Modula" in the list
- If update is available, click "Update"