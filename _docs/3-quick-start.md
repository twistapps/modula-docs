---
title: Quick Start
permalink: /quick-start
excerpt: "How to take off fast!"

author_profile: false
author: Twist Apps

#toc: false

#classes: wide

---

After [adding Modula to your project](/install), it's time to make your first module!

#### Making example behaviour

**Step 1** - create new _[main script](/module-features#main-)_ that supports modules:
- Create new MonoBehaviour script
- use namespace `Modula`
- change inheritance to `ModularBehaviour`

{% highlight C# %}using Modula;


public class ModularExample : ModularBehaviour
{

}{% endhighlight %}

**Step 2** - create your first _module_
- Create new MonoBehaviour script
- use namespace `Modula`
- change inheritance to `Module`

{% highlight C# %}using Modula;


public class ExampleModule : Module
{

}{% endhighlight %}

**Step 3** - add support for `ExampleModule` in `ModularExample`
- Get back to your behaviour script
- Override `AvailableModules` field

{% highlight C# %}
public class ModularExample : ModularBehaviour
{
    public override TypeList AvailableModules { get; } 
        = new TypeList()
        .Add(typeof(ExampleModule));
}{% endhighlight %}

**Step 4** - create GameObject for your new behaviour
- in Unity, go to Hierarchy window > "+" > Create Empty
- select the created object
- click "Add Component" > ModularExample

**Done!** now you can add or remove your module in Inspector window by clicking
"Add ExampleModule" / "Remove"
{: .notice--success }

#### Result
![result image](/assets/img/modular-example.gif)
{: .notice}