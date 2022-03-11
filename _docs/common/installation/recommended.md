﻿
**There are [multiple ways](/install)** to install Modula.<br>
We recommend using it as [Unity Package Manager (UPM)](https://docs.unity3d.com/Manual/upm-ui.html) Git dependency:
{: .notice--info}
### 1. Recommended Method `(UPM Git Dependency)`
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