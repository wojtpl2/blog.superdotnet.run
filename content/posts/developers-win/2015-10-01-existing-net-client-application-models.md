---
title: Existing .NET Client Application Models
author: Mike-EEE
type: post
date: 2015-10-01T20:06:07+00:00
excerpt: 'The Bridge to .NET Ubiquity: Existing .NET Client Application Models. In this article, we explore the known .NET client application models, and see how they stack up against our list of desired qualities in a ubiquitous .NET client application.'
url: /2015/10/existing-net-client-application-models/
featured_image: /wp-content/uploads/2015/09/Transpile.png
mythemes-thumbnail-height:
  - 45
dsq_thread_id:
  - 4158325163
sponge:
  - 1
sandpaper:
  - 1
categories:
  - Developers-Win
  - General
series:
  - The Bridge to .NET Ubiquity

---
<div class="seriesmeta">
  This entry is part 3 of 6 in the series <a href="/series/bridge-to-dotnet-ubiquity/" class="series-6" title="The Bridge to .NET Ubiquity">The Bridge to .NET Ubiquity</a>
</div>

### TL;DR: VOTE!

This series exists to build support around the idea of a ubiquitous .NET client application development model. This is not intended to be a final solution, but a starting point for discussion, awareness, and a sign of demand. Show your support by voting for this idea here:

<div class="push-button-container"><div class="push-button">
</div><a class="w-inline-block top-lighting" href="http://visualstudio.uservoice.com/forums/121579-visual-studio/suggestions/10027638-create-a-ubiquitous-net-client-application-develo" target="_blank"><div class="glass-insert" data-ix="blink" style="transition: opacity 500ms ease-in-out; opacity: 0;"></div><img class="push-button-vote-text" src="/images/VoteNow.svg" /></a></div>

### .NET Client Application Models

In this post, [we][1] outline all the known .NET client application models and compare them with [the list of qualities][2] we feel are necessary for a truly ubiquitous .NET client application model. As we will demonstrate on a case-by-case basis, each model below possesses one or more qualities, but no one single model possesses them all. It is through this exercise of compare-and-contrast that we hope to accurately outline what a ubiquitous .NET client application looks like, as well as provide a window into the frustrating search of successfully finding a ubiquitous .NET client application model in today&#8217;s market. We have broken the different models into two different types: compiled (native platform) client application models and web-based client application models, and start with the compiled models first.

_(With each client application model below, we have denoted <span style="color: #95c11f;">matched ubiquitous qualities in green icons</span> and <span style="color: #ce2f18;">unmatched ubiquitous qualities in red icons</span>.)_

## Compiled (Native or Store-Hosted) Client Application Models

### Windows Forms

<div class="icon-container">
  <a class="w-inline-block qualityicon cross-platform-icon red" href="/2015/10/ubiquitous-qualities/#native-cross-platform-capable" target="_blank" data-ix="cross-platform-hover"> 
  
  <div class="cross-platform">
    <div class="overlay-container red">
      <div class="overlay-text">
        NATIVE <br />CROSS-PLATFORM <br />CAPABLE
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon html5-icon red" href="/2015/10/ubiquitous-qualities/#html5-compliant" target="_blank" data-ix="html5-hover"> 
  
  <div class="html5-compliant">
    <div class="overlay-container red">
      <div class="overlay-text">
        HTML5 <br />COMPLIANT
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon ux-icon green" href="/2015/10/ubiquitous-qualities/#consistent-user-experience" target="_blank" data-ix="ux-hover"> 
  
  <div class="consistent-ux">
    <div class="overlay-container green">
      <div class="overlay-text">
        CONSISTENT <br />USER <br />EXPERIENCE
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon cross-boundary-icon green" href="/2015/10/ubiquitous-qualities/#cross-boundary-accessibility" target="_blank" data-ix="cross-boundary-hover"> 
  
  <div class="cross-boundary">
    <div class="overlay-container green">
      <div class="overlay-text">
        CROSS-BOUNDARY <br />Accessibility
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon xaml-icon red" href="/2015/10/ubiquitous-qualities/#xaml-powered" target="_blank" data-ix="xaml-hover"> 
  
  <div class="xaml-driven">
    <div class="overlay-container red">
      <div class="overlay-text">
        XAML-POWERED
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon object-congruence-icon green" href="/2015/10/ubiquitous-qualities/#object-serialization-congruence" target="_blank" data-ix="congruence-hover"> 
  
  <div class="object-congruence">
    <div class="overlay-container green">
      <div class="overlay-text">
        OBJECT <br />SERIALIZATION <br />CONGRUENCE
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon holistic-dev-icon green" href="/2015/10/ubiquitous-qualities/#holistic-development-consistency" target="_blank" data-ix="holistic-dev-hover"> 
  
  <div class="holistic-dev">
    <div class="overlay-container green">
      <div class="overlay-text">
        HOLISTIC <br />DEVELOPMENT <br />CONSISTENCY
      </div>
    </div>
  </div></a>
</div>

We start with <a href="https://msdn.microsoft.com/en-us/library/dd30h2yb%28v=vs.110%29.aspx?f=255&#038;MSPPError=-2147217396" target="_blank" rel="noopener">Windows Forms</a>. Windows Forms can be considered the first .NET client application model and (surprisingly) still pulls weight today in the world of line of business applications. There is even <a href="https://visualstudio.uservoice.com/forums/121579-visual-studio/suggestions/8127717-open-source-windows-forms" target="_blank" rel="noopener">an outstanding vote with considerable backing to make it open source</a>. As this was the first .NET client application model, it did lead the way with the concept of a designer-friendly tooling paradigm. However, the designer was not based on a serialization mechanism and this led to a lot of code being generated instead, leading developers to mark this as a negative aspect of Windows Forms development. In fact, it is safe to say that this aspect is what led to a more robust, readable, and manageable solution found within its successor and the next model we will visit. As Windows Forms was built with the first version of .NET, it was inherently Windows-only, with no chance of cross-platform capability. However, as a native .NET client application model, it does benefit from the holistic development consistency that occurs when being a part of a .NET solution, as well as shared components and assemblies between application boundaries.</p> 


### Windows Presentation Foundation

<div class="icon-container">
  <a class="w-inline-block qualityicon cross-platform-icon red" href="/2015/10/ubiquitous-qualities/#native-cross-platform-capable" target="_blank" data-ix="cross-platform-hover"> 
  
  <div class="cross-platform">
    <div class="overlay-container red">
      <div class="overlay-text">
        NATIVE <br />CROSS-PLATFORM <br />CAPABLE
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon html5-icon red" href="/2015/10/ubiquitous-qualities/#html5-compliant" target="_blank" data-ix="html5-hover"> 
  
  <div class="html5-compliant">
    <div class="overlay-container red">
      <div class="overlay-text">
        HTML5 <br />COMPLIANT
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon ux-icon green" href="/2015/10/ubiquitous-qualities/#consistent-user-experience" target="_blank" data-ix="ux-hover"> 
  
  <div class="consistent-ux">
    <div class="overlay-container green">
      <div class="overlay-text">
        CONSISTENT <br />USER <br />EXPERIENCE
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon cross-boundary-icon green" href="/2015/10/ubiquitous-qualities/#cross-boundary-accessibility" target="_blank" data-ix="cross-boundary-hover"> 
  
  <div class="cross-boundary">
    <div class="overlay-container green">
      <div class="overlay-text">
        CROSS-BOUNDARY <br />Accessibility
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon xaml-icon green" href="/2015/10/ubiquitous-qualities/#xaml-powered" target="_blank" data-ix="xaml-hover"> 
  
  <div class="xaml-driven">
    <div class="overlay-container green">
      <div class="overlay-text">
        XAML-POWERED
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon object-congruence-icon green" href="/2015/10/ubiquitous-qualities/#object-serialization-congruence" target="_blank" data-ix="congruence-hover"> 
  
  <div class="object-congruence">
    <div class="overlay-container green">
      <div class="overlay-text">
        OBJECT <br />SERIALIZATION <br />CONGRUENCE
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon holistic-dev-icon green" href="/2015/10/ubiquitous-qualities/#holistic-development-consistency" target="_blank" data-ix="holistic-dev-hover"> 
  
  <div class="holistic-dev">
    <div class="overlay-container green">
      <div class="overlay-text">
        HOLISTIC <br />DEVELOPMENT <br />CONSISTENCY
      </div>
    </div>
  </div></a>
</div>

The big daddy of .NET application client models.  

<a href="https://msdn.microsoft.com/en-us/library/ms754130(v=vs.110).aspx" target="_blank" rel="noopener">Windows Presentation Foundation</a> (WPF) was simply an outstanding innovation in Microsoft client application technology, and can be considered the de facto standard for any .NET client application model. WPF was innovative in many areas, but primarily in how it enabled serialization and design through the use of a new technology known as <a href="https://msdn.microsoft.com/en-us/library/cc295302.aspx" target="_blank" rel="noopener">Xaml</a>. Xaml is an object description technology that is based off of XML. When WPF was first introduced, Xaml was strictly for defining and describing user interface elements. In later versions, this power got abstracted into its own assembly with System.Xaml, where it lives today and other frameworks such as <a href="https://msdn.microsoft.com/en-us/library/ee342461.aspx" target="_blank" rel="noopener">Windows Workflow</a> utilize it. WPF has it all except for cross-platform and web compatibility. In fact, this very shortcoming is what led Microsoft on another endeavor to bring the power of WPF to the web, known as Silverlight.</p> 

### Silverlight

<div class="icon-container">
  <a class="w-inline-block qualityicon cross-platform-icon red" href="/2015/10/ubiquitous-qualities/#native-cross-platform-capable" target="_blank" data-ix="cross-platform-hover"> 
  
  <div class="cross-platform">
    <div class="overlay-container red">
      <div class="overlay-text">
        NATIVE <br />CROSS-PLATFORM <br />CAPABLE
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon html5-icon red" href="/2015/10/ubiquitous-qualities/#html5-compliant" target="_blank" data-ix="html5-hover"> 
  
  <div class="html5-compliant">
    <div class="overlay-container red">
      <div class="overlay-text">
        HTML5 <br />COMPLIANT
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon ux-icon green" href="/2015/10/ubiquitous-qualities/#consistent-user-experience" target="_blank" data-ix="ux-hover"> 
  
  <div class="consistent-ux">
    <div class="overlay-container green">
      <div class="overlay-text">
        CONSISTENT <br />USER <br />EXPERIENCE
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon cross-boundary-icon green" href="/2015/10/ubiquitous-qualities/#cross-boundary-accessibility" target="_blank" data-ix="cross-boundary-hover"> 
  
  <div class="cross-boundary">
    <div class="overlay-container green">
      <div class="overlay-text">
        CROSS-BOUNDARY <br />Accessibility
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon xaml-icon green" href="/2015/10/ubiquitous-qualities/#xaml-powered" target="_blank" data-ix="xaml-hover"> 
  
  <div class="xaml-driven">
    <div class="overlay-container green">
      <div class="overlay-text">
        XAML-POWERED
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon object-congruence-icon green" href="/2015/10/ubiquitous-qualities/#object-serialization-congruence" target="_blank" data-ix="congruence-hover"> 
  
  <div class="object-congruence">
    <div class="overlay-container green">
      <div class="overlay-text">
        OBJECT <br />SERIALIZATION <br />CONGRUENCE
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon holistic-dev-icon green" href="/2015/10/ubiquitous-qualities/#holistic-development-consistency" target="_blank" data-ix="holistic-dev-hover"> 
  
  <div class="holistic-dev">
    <div class="overlay-container green">
      <div class="overlay-text">
        HOLISTIC <br />DEVELOPMENT <br />CONSISTENCY
      </div>
    </div>
  </div></a>
</div>

<a href="http://www.microsoft.com/silverlight/what-is-silverlight/" target="_blank" rel="noopener">Silverlight </a>is probably the most controversial, misrepresented, mis-marketed, and misunderstood product in Microsoft&#8217;s history. _**To date, Silverlight is the closest match to a ubiquitous .NET client application model that Microsoft has ever created.**_ To the developers who loved it, it was a ported subset of WPF, a .NET client application model, enabled to live in a browser in a cross-platform way. To everyone else, it was a disruptive plugin that required installation on the users machine to operate correctly. Silverlight was a very polarizing force and you either hated it as pure web developers did or loved it as pure Microsoft .NET developers did. At the time it was created, Silverlight was a (very) unique Microsoft property in that enabled .NET applications to run on a Macintosh. However, when the device revolution occurred, Apple disallowed plugins to run on their iOS devices (and browsers running on them), and <a href="http://www.zdnet.com/article/microsoft-our-strategy-with-silverlight-has-shifted/" target="_blank" rel="noopener">Silverlight met a most confusing and mismanaged death</a>. Technically, it is still supported today until 2021, but most Silverlight developers have moved on to other client models, while commonly regaling its power and elegance in various (and random) forum and blog posts.</p> 

### Universal Windows Platform

<div class="icon-container">
  <a class="w-inline-block qualityicon cross-platform-icon red" href="/2015/10/ubiquitous-qualities/#native-cross-platform-capable" target="_blank" data-ix="cross-platform-hover"> 
  
  <div class="cross-platform">
    <div class="overlay-container red">
      <div class="overlay-text">
        NATIVE <br />CROSS-PLATFORM <br />CAPABLE
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon html5-icon red" href="/2015/10/ubiquitous-qualities/#html5-compliant" target="_blank" data-ix="html5-hover"> 
  
  <div class="html5-compliant">
    <div class="overlay-container red">
      <div class="overlay-text">
        HTML5 <br />COMPLIANT
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon ux-icon green" href="/2015/10/ubiquitous-qualities/#consistent-user-experience" target="_blank" data-ix="ux-hover"> 
  
  <div class="consistent-ux">
    <div class="overlay-container green">
      <div class="overlay-text">
        CONSISTENT <br />USER <br />EXPERIENCE
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon cross-boundary-icon green" href="/2015/10/ubiquitous-qualities/#cross-boundary-accessibility" target="_blank" data-ix="cross-boundary-hover"> 
  
  <div class="cross-boundary">
    <div class="overlay-container green">
      <div class="overlay-text">
        CROSS-BOUNDARY <br />Accessibility
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon xaml-icon red" href="/2015/10/ubiquitous-qualities/#xaml-powered" target="_blank" data-ix="xaml-hover"> 
  
  <div class="xaml-driven">
    <div class="overlay-container red">
      <div class="overlay-text">
        XAML-POWERED
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon object-congruence-icon green" href="/2015/10/ubiquitous-qualities/#object-serialization-congruence" target="_blank" data-ix="congruence-hover"> 
  
  <div class="object-congruence">
    <div class="overlay-container green">
      <div class="overlay-text">
        OBJECT <br />SERIALIZATION <br />CONGRUENCE
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon holistic-dev-icon green" href="/2015/10/ubiquitous-qualities/#holistic-development-consistency" target="_blank" data-ix="holistic-dev-hover"> 
  
  <div class="holistic-dev">
    <div class="overlay-container green">
      <div class="overlay-text">
        HOLISTIC <br />DEVELOPMENT <br />CONSISTENCY
      </div>
    </div>
  </div></a>
</div> The 

<a href="https://msdn.microsoft.com/en-us/library/windows/apps/dn894631.aspx" target="_blank" rel="noopener">Universal Windows Platform</a> (UWP) is the latest .NET client application model offering from Microsoft, and it can be considered a &#8220;complimentary replacement&#8221; to WPF. If you find that term confusing, then it has done its job. UWP (formerly known as Windows Runtime, or WinRT) was designed alongside WPF in a completely different runtime, and was intended to mimic (read: catch up to) Apple and Google by introducing a central application store, where UWP applications can be deployed to and installed by consumers.</p> 

Although technically .NET, UWP is designed around an exhaustive set of interfaces that ultimately lead to implementations developed in C++ and COM code. This has been called the &#8220;**Curtain of COM**&#8221; and has led to a very different development experience for .NET developers in the UWP environment. The Curtain of COM can be considered an application boundary in its own right. Errors thrown from the there are usually obscure at best, and when an event does arise from it, very little information can be derived from the call stack or other (usually helpful) debugging contexts, which in comparison to WPF and traditional .NET development are usually loaded with rich debugging information.

UWP has been out for several years now, but it still suffers from some serious drawbacks. In addition to the opaque Curtain of COM described above, UWP has a very limited Xaml system that hardly reflects the power of Xaml as seen in WPF or even Silverlight 5. Additionally, whereas much effort was made to make Xaml generalized and abstract in WPF and Silverlight 5, UWP reversed all efforts there by making Xaml a concern of the user interface again. The power of Xaml is in its serialization capability, and also in its markup extensions, both of which are absent in UWP Xaml. _Because of this, we do not consider UWP to meet our requirements for a Xaml-powered client application model._

In addition to the dreaded Curtain of COM and a weak Xaml model, UWP does not enable the most fundamental .NET principles and design by way of language support. .NET was designed and intended to allow developers to design their applications in their most preferred language. <a href="https://wpdev.uservoice.com/forums/110705-universal-windows-platform/suggestions/9110134-f-support-in-net-native-for-uwp" target="_blank" rel="noopener">UWP still does not support F#</a>, which is really a tremendous and embarrassing failing for this group.

Despite these shortcomings, UWP does introduce the concept of a packaged application that is deployed to the <a href="http://windows.microsoft.com/en-us/windows-8/apps-windows-store-tutorial" target="_blank" rel="noopener">Windows Store</a>. This is a very powerful (and well-executed) concept in its ecosystem, as commerce can easily occur not only in sale of applications, but also within the applications it hosts as well. UWP provides the APIs to enable this new form of monetary exchange that was not and is not in WPF. However, even given this highlight, the choice was made to make UWP a Windows-only endeavor, foregoing the cross-platform capability and promise that Silverlight attempted to deliver. In summary, UWP has many challenges to overcome before being considered a candidate for a ubiquitous .NET client application model.

### Xamarin.Forms

<div class="icon-container">
  <a class="w-inline-block qualityicon cross-platform-icon green" href="/2015/10/ubiquitous-qualities/#native-cross-platform-capable" target="_blank" data-ix="cross-platform-hover"> 
  
  <div class="cross-platform">
    <div class="overlay-container green">
      <div class="overlay-text">
        NATIVE <br />CROSS-PLATFORM <br />CAPABLE
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon html5-icon red" href="/2015/10/ubiquitous-qualities/#html5-compliant" target="_blank" data-ix="html5-hover"> 
  
  <div class="html5-compliant">
    <div class="overlay-container red">
      <div class="overlay-text">
        HTML5 <br />COMPLIANT
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon ux-icon red" href="/2015/10/ubiquitous-qualities/#consistent-user-experience" target="_blank" data-ix="ux-hover"> 
  
  <div class="consistent-ux">
    <div class="overlay-container red">
      <div class="overlay-text">
        CONSISTENT <br />USER <br />EXPERIENCE
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon cross-boundary-icon green" href="/2015/10/ubiquitous-qualities/#cross-boundary-accessibility" target="_blank" data-ix="cross-boundary-hover"> 
  
  <div class="cross-boundary">
    <div class="overlay-container green">
      <div class="overlay-text">
        CROSS-BOUNDARY <br />Accessibility
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon xaml-icon green" href="/2015/10/ubiquitous-qualities/#xaml-powered" target="_blank" data-ix="xaml-hover"> 
  
  <div class="xaml-driven">
    <div class="overlay-container green">
      <div class="overlay-text">
        XAML-POWERED
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon object-congruence-icon green" href="/2015/10/ubiquitous-qualities/#object-serialization-congruence" target="_blank" data-ix="congruence-hover"> 
  
  <div class="object-congruence">
    <div class="overlay-container green">
      <div class="overlay-text">
        OBJECT <br />SERIALIZATION <br />CONGRUENCE
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon holistic-dev-icon green" href="/2015/10/ubiquitous-qualities/#holistic-development-consistency" target="_blank" data-ix="holistic-dev-hover"> 
  
  <div class="holistic-dev">
    <div class="overlay-container green">
      <div class="overlay-text">
        HOLISTIC <br />DEVELOPMENT <br />CONSISTENCY
      </div>
    </div>
  </div></a>
</div>

<a href="https://xamarin.com/forms" target="_blank" rel="noopener">Xamarin.Forms</a> is considered the new .NET client application on the block, and offers good promise to be a ubiquitous .NET client application model in the future. Created by <a href="https://xamarin.com" target="_blank" rel="noopener">Xamarin</a>, an external company and now <a href="https://blog.xamarin.com/microsoft-and-xamarin-expand-global-partnership/" target="_blank" rel="noopener">strategic partner of Microsoft</a>, Xamarin.Forms offers a Xaml model that is (ironically) better designed and more powerful than UWP&#8217;s. Xamarin.Forms works on iOS, Droid, and Windows, fully possessing the quality for cross-platform compatibility.</p> 

However, even though Xamarin.Forms&#8217; client application model is fully cross-platform, its client application model is an adaptive one. An _adaptive client application model_ adapts to the hosting environment it executes on, and renders the user interface elements and subsequent user experience that is native to that host. Because of this, Xamarin.Forms does not have a consistent user experience across different devices on different platforms, and failing to meet our ubiquitous .NET client application model requirement for consistent user experience.

Additionally &#8212; and more unfortunate &#8212; Xamarin.Forms does not provide a HTML5-compliant offering, failing another important requirement in our list of desired qualites. Even so, Xamarin.Forms is still an impressive technology and Xamarin is even more so an impressive company and strategic partner to Microsoft. It says something when an external partner understands a technology (Xaml) better than the company that made it, as seen when comparing Xamarin&#8217;s Xaml model to the one found in UWP. There is definitely a feeling that this partnership could and should be leveraged in any endeavor to create a ubiquitous .NET client application model.

### Avalonia

<div class="icon-container">
  <a class="w-inline-block qualityicon cross-platform-icon green" href="/2015/10/ubiquitous-qualities/#native-cross-platform-capable" target="_blank" data-ix="cross-platform-hover"> 
  
  <div class="cross-platform">
    <div class="overlay-container green">
      <div class="overlay-text">
        NATIVE <br />CROSS-PLATFORM <br />CAPABLE
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon html5-icon red" href="/2015/10/ubiquitous-qualities/#html5-compliant" target="_blank" data-ix="html5-hover"> 
  
  <div class="html5-compliant">
    <div class="overlay-container red">
      <div class="overlay-text">
        HTML5 <br />COMPLIANT
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon ux-icon green" href="/2015/10/ubiquitous-qualities/#consistent-user-experience" target="_blank" data-ix="ux-hover"> 
  
  <div class="consistent-ux">
    <div class="overlay-container green">
      <div class="overlay-text">
        CONSISTENT <br />USER <br />EXPERIENCE
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon cross-boundary-icon green" href="/2015/10/ubiquitous-qualities/#cross-boundary-accessibility" target="_blank" data-ix="cross-boundary-hover"> 
  
  <div class="cross-boundary">
    <div class="overlay-container green">
      <div class="overlay-text">
        CROSS-BOUNDARY <br />Accessibility
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon xaml-icon green" href="/2015/10/ubiquitous-qualities/#xaml-powered" target="_blank" data-ix="xaml-hover"> 
  
  <div class="xaml-driven">
    <div class="overlay-container green">
      <div class="overlay-text">
        XAML-POWERED
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon object-congruence-icon green" href="/2015/10/ubiquitous-qualities/#object-serialization-congruence" target="_blank" data-ix="congruence-hover"> 
  
  <div class="object-congruence">
    <div class="overlay-container green">
      <div class="overlay-text">
        OBJECT <br />SERIALIZATION <br />CONGRUENCE
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon holistic-dev-icon green" href="/2015/10/ubiquitous-qualities/#holistic-development-consistency" target="_blank" data-ix="holistic-dev-hover"> 
  
  <div class="holistic-dev">
    <div class="overlay-container green">
      <div class="overlay-text">
        HOLISTIC <br />DEVELOPMENT <br />CONSISTENCY
      </div>
    </div>
  </div></a>
</div>

<a href="https://github.com/AvaloniaUI/Avalonia" target="_blank" rel="noopener">Avalonia</a> is a new-comer to the game and is currently lighting up the field in spectacular fashion. It is just getting off the ground and is showing a lot of promise. Avalonia is currently running in alpha, and allows Xaml-based designer support and an inspector for your processed/loaded Xaml. It is also powered by a much needed cross-platform Xaml parser known as <a href="https://github.com/SuperJMN/OmniXAML" target="_blank" rel="noopener">OmniXaml</a>. Avalonia currently runs in *nix and Macintosh, but not in Droid or iOS (yet). However, they are currently exploring MonoGame support which would enable these scenarios. Avalonia does not currently offer a transpiled offering into JavaScript artifacts, so these scenarios are currently prohibitive and does not meet our requirement for HTML5-compliance. However, the group around this project seem very in-tune and capable, and we expect this project to go places.</p> 

### Urho3D

<div class="icon-container">
  <a class="w-inline-block qualityicon cross-platform-icon green" href="/2015/10/ubiquitous-qualities/#native-cross-platform-capable" target="_blank" data-ix="cross-platform-hover"> 
  
  <div class="cross-platform">
    <div class="overlay-container green">
      <div class="overlay-text">
        NATIVE <br />CROSS-PLATFORM <br />CAPABLE
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon html5-icon red" href="/2015/10/ubiquitous-qualities/#html5-compliant" target="_blank" data-ix="html5-hover"> 
  
  <div class="html5-compliant">
    <div class="overlay-container red">
      <div class="overlay-text">
        HTML5 <br />COMPLIANT
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon ux-icon green" href="/2015/10/ubiquitous-qualities/#consistent-user-experience" target="_blank" data-ix="ux-hover"> 
  
  <div class="consistent-ux">
    <div class="overlay-container green">
      <div class="overlay-text">
        CONSISTENT <br />USER <br />EXPERIENCE
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon cross-boundary-icon green" href="/2015/10/ubiquitous-qualities/#cross-boundary-accessibility" target="_blank" data-ix="cross-boundary-hover"> 
  
  <div class="cross-boundary">
    <div class="overlay-container green">
      <div class="overlay-text">
        CROSS-BOUNDARY <br />Accessibility
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon xaml-icon red" href="/2015/10/ubiquitous-qualities/#xaml-powered" target="_blank" data-ix="xaml-hover"> 
  
  <div class="xaml-driven">
    <div class="overlay-container red">
      <div class="overlay-text">
        XAML-POWERED
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon object-congruence-icon green" href="/2015/10/ubiquitous-qualities/#object-serialization-congruence" target="_blank" data-ix="congruence-hover"> 
  
  <div class="object-congruence">
    <div class="overlay-container green">
      <div class="overlay-text">
        OBJECT <br />SERIALIZATION <br />CONGRUENCE
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon holistic-dev-icon green" href="/2015/10/ubiquitous-qualities/#holistic-development-consistency" target="_blank" data-ix="holistic-dev-hover"> 
  
  <div class="holistic-dev">
    <div class="overlay-container green">
      <div class="overlay-text">
        HOLISTIC <br />DEVELOPMENT <br />CONSISTENCY
      </div>
    </div>
  </div></a>
</div>

[Urho3D][3] is a 3D gaming engine that has its own user interface subsystem, and <a href="https://blog.xamarin.com/3d-game-engine-for-android-ios-and-net/" target="_blank" rel="noopener">was recently made available to .NET</a> from the good folks at <a href="http://xamarin.com" target="_blank" rel="noopener">Xamarin</a>. Like Xamarin.Forms, Urho3D enables .NET application development for iOS, Android, and Mac. Urho3D could be seen as a viable, recommended replacement for Monogame, or at least the official cross-platform 3D .NET application recommendation from Xamarin. We list Urho3D here rather than <a href="http://monogame.net" target="_blank" rel="noopener">Monogame </a>as it does have its own <a href="http://urho3d.github.io/documentation/1.5/class_urho3_d_1_1_u_i.html" target="_blank" rel="noopener">user interface subsystem</a>, which makes it possible to define a client application model as such.</p> 

Unfortunately, Urho3D does not support Xaml (at the moment) and while <a href="http://urho3d.github.io/HTML5-samples.html" target="_blank" rel="noopener">it does have support for creating transpiled HTML5 output via its C++ offering</a>, this is not possible via the .NET offering from Xamarin as it is based on the same technology toolchain as Xamarin.Forms. However, since it does have its own user interface subsystem, Urho3D does meet the <a href="/2015/10/ubiquitous-qualities/#consistent-user-experience" target="_blank" rel="noopener">consistent user interface and experience requirement</a> that Xamarin.Forms does not.

### x2h: Xaml-to-Html Translator

<div class="icon-container">
  <a class="w-inline-block qualityicon cross-platform-icon red" href="/2015/10/ubiquitous-qualities/#native-cross-platform-capable" target="_blank" data-ix="cross-platform-hover"> 
  
  <div class="cross-platform">
    <div class="overlay-container red">
      <div class="overlay-text">
        NATIVE <br />CROSS-PLATFORM <br />CAPABLE
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon html5-icon green" href="/2015/10/ubiquitous-qualities/#html5-compliant" target="_blank" data-ix="html5-hover"> 
  
  <div class="html5-compliant">
    <div class="overlay-container green">
      <div class="overlay-text">
        HTML5 <br />COMPLIANT
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon ux-icon red" href="/2015/10/ubiquitous-qualities/#consistent-user-experience" target="_blank" data-ix="ux-hover"> 
  
  <div class="consistent-ux">
    <div class="overlay-container red">
      <div class="overlay-text">
        CONSISTENT <br />USER <br />EXPERIENCE
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon cross-boundary-icon red" href="/2015/10/ubiquitous-qualities/#cross-boundary-accessibility" target="_blank" data-ix="cross-boundary-hover"> 
  
  <div class="cross-boundary">
    <div class="overlay-container red">
      <div class="overlay-text">
        CROSS-BOUNDARY <br />Accessibility
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon xaml-icon green" href="/2015/10/ubiquitous-qualities/#xaml-powered" target="_blank" data-ix="xaml-hover"> 
  
  <div class="xaml-driven">
    <div class="overlay-container green">
      <div class="overlay-text">
        XAML-POWERED
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon object-congruence-icon green" href="/2015/10/ubiquitous-qualities/#object-serialization-congruence" target="_blank" data-ix="congruence-hover"> 
  
  <div class="object-congruence">
    <div class="overlay-container green">
      <div class="overlay-text">
        OBJECT <br />SERIALIZATION <br />CONGRUENCE
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon holistic-dev-icon green" href="/2015/10/ubiquitous-qualities/#holistic-development-consistency" target="_blank" data-ix="holistic-dev-hover"> 
  
  <div class="holistic-dev">
    <div class="overlay-container green">
      <div class="overlay-text">
        HOLISTIC <br />DEVELOPMENT <br />CONSISTENCY
      </div>
    </div>
  </div></a>
</div>

Have you ever seen the request on a forum post or blog comment that &#8220;someone should build a converter for Xaml to HTML output?&#8221; If you visit any of the MSDN forums, blogs or UserVoice boards, you have probably seen it a lot. Well, someone has done exactly that in <a href="http://xaml2html.net/" target="_blank" rel="noopener">xaml2html</a>. It has just been released as a beta for developers to try out. As it is new it is very raw, but the working concept shows that it is possible to take a WPF project and output its contents and &#8220;translate&#8221; them into another form &#8212; HTML5-compliant artifacts, to be exact. Do note that this is more of a technology/project than an client application development model, but it is worth knowing about and to follow along with its progress to see how it evolves.</p> 

### Azure PowerApps

<div class="icon-container">
  <a class="w-inline-block qualityicon cross-platform-icon green" href="/2015/10/ubiquitous-qualities/#native-cross-platform-capable" target="_blank" data-ix="cross-platform-hover"> 
  
  <div class="cross-platform">
    <div class="overlay-container green">
      <div class="overlay-text">
        NATIVE <br />CROSS-PLATFORM <br />CAPABLE
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon html5-icon green" href="/2015/10/ubiquitous-qualities/#html5-compliant" target="_blank" data-ix="html5-hover"> 
  
  <div class="html5-compliant">
    <div class="overlay-container green">
      <div class="overlay-text">
        HTML5 <br />COMPLIANT
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon ux-icon green" href="/2015/10/ubiquitous-qualities/#consistent-user-experience" target="_blank" data-ix="ux-hover"> 
  
  <div class="consistent-ux">
    <div class="overlay-container green">
      <div class="overlay-text">
        CONSISTENT <br />USER <br />EXPERIENCE
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon cross-boundary-icon red" href="/2015/10/ubiquitous-qualities/#cross-boundary-accessibility" target="_blank" data-ix="cross-boundary-hover"> 
  
  <div class="cross-boundary">
    <div class="overlay-container red">
      <div class="overlay-text">
        CROSS-BOUNDARY <br />Accessibility
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon xaml-icon red" href="/2015/10/ubiquitous-qualities/#xaml-powered" target="_blank" data-ix="xaml-hover"> 
  
  <div class="xaml-driven">
    <div class="overlay-container red">
      <div class="overlay-text">
        XAML-POWERED
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon object-congruence-icon red" href="/2015/10/ubiquitous-qualities/#object-serialization-congruence" target="_blank" data-ix="congruence-hover"> 
  
  <div class="object-congruence">
    <div class="overlay-container red">
      <div class="overlay-text">
        OBJECT <br />SERIALIZATION <br />CONGRUENCE
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon holistic-dev-icon red" href="/2015/10/ubiquitous-qualities/#holistic-development-consistency" target="_blank" data-ix="holistic-dev-hover"> 
  
  <div class="holistic-dev">
    <div class="overlay-container red">
      <div class="overlay-text">
        HOLISTIC <br />DEVELOPMENT <br />CONSISTENCY
      </div>
    </div>
  </div></a>
</div>

[Azure PowerApps][4] is a product that is in preview, and holds some promise in the search of a ubiquitous client application model. It has cross platform capabilities, working on iOS, Droid, Windows Store, and the web. As promising as this sounds, its intended audience at moment is the non-professional developer, working on internal corporate line-of-business applications (think: next generation Excel macro-maker). This obviously prohibits professional .NET developers (at present) from developing consumer applications with this model, but it will be interesting to watch going forward if this does move towards this space. Considering that this is coming out of the Azure group, this product has every reason in the world to succeed and become a viable force in the marketplace. For more information on this exciting, emerging technology, <a href="https://blogs.msdn.microsoft.com/azuredev/2016/02/14/playing-with-power-powerapps/" target="_blank" rel="noopener">check out Mike-EEE&#8217;s guest article on the MSDN Azure Development Blog</a>.</p> 

### Azure RemoteApp

<div class="icon-container">
  <a class="w-inline-block qualityicon cross-platform-icon green" href="/2015/10/ubiquitous-qualities/#native-cross-platform-capable" target="_blank" data-ix="cross-platform-hover"> 
  
  <div class="cross-platform">
    <div class="overlay-container green">
      <div class="overlay-text">
        NATIVE <br />CROSS-PLATFORM <br />CAPABLE
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon html5-icon red" href="/2015/10/ubiquitous-qualities/#html5-compliant" target="_blank" data-ix="html5-hover"> 
  
  <div class="html5-compliant">
    <div class="overlay-container red">
      <div class="overlay-text">
        HTML5 <br />COMPLIANT
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon ux-icon green" href="/2015/10/ubiquitous-qualities/#consistent-user-experience" target="_blank" data-ix="ux-hover"> 
  
  <div class="consistent-ux">
    <div class="overlay-container green">
      <div class="overlay-text">
        CONSISTENT <br />USER <br />EXPERIENCE
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon cross-boundary-icon green" href="/2015/10/ubiquitous-qualities/#cross-boundary-accessibility" target="_blank" data-ix="cross-boundary-hover"> 
  
  <div class="cross-boundary">
    <div class="overlay-container green">
      <div class="overlay-text">
        CROSS-BOUNDARY <br />Accessibility
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon xaml-icon green" href="/2015/10/ubiquitous-qualities/#xaml-powered" target="_blank" data-ix="xaml-hover"> 
  
  <div class="xaml-driven">
    <div class="overlay-container green">
      <div class="overlay-text">
        XAML-POWERED
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon object-congruence-icon green" href="/2015/10/ubiquitous-qualities/#object-serialization-congruence" target="_blank" data-ix="congruence-hover"> 
  
  <div class="object-congruence">
    <div class="overlay-container green">
      <div class="overlay-text">
        OBJECT <br />SERIALIZATION <br />CONGRUENCE
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon holistic-dev-icon green" href="/2015/10/ubiquitous-qualities/#holistic-development-consistency" target="_blank" data-ix="holistic-dev-hover"> 
  
  <div class="holistic-dev">
    <div class="overlay-container green">
      <div class="overlay-text">
        HOLISTIC <br />DEVELOPMENT <br />CONSISTENCY
      </div>
    </div>
  </div></a>
</div> Finally, we end our tour through native-hosted client application models with a technology from 

<a href="https://azure.microsoft.com/" target="_blank" rel="noopener">Azure</a>, known as <a href="https://azure.microsoft.com/en-us/documentation/videos/azure-remoteapp-cloud-deployment-overview/" target="_blank" rel="noopener">RemoteApp</a>. To be sure, RemoteApp is more of a technology than a client application model &#8212; you can think of it as a client application model _host_. Using Remote Desktop technology, RemoteApp will take a Windows application installed on Azure and feed its rendering to a user&#8217;s remote device. That device can be a iOS, Droid, and of course a Windows device. Since it can be any Windows application, a developer could use WPF and have full access to its power and Xaml engine.</p> 

Currently, RemoteApp is meant for enterprise scenarios, and it would be interesting to see if there are plans to make it more for consumer-based scenarios. Additionally, while it only currently supports native-hosted applications, it would be interesting to see if RemoteApp could be used to pipe its renderings through a WebGL canvas on an HTML5 web page to <a href="/2015/10/ubiquitous-qualities/#html5-compliant" target="_blank" rel="noopener">fulfill our HTML5-Compliant Requirement</a>.

While RemoteApp offers a lot of promise, there are some considerations. First, if this technology branched out to the consumer space, there is no telling how feasibly scalable it would be. RemoteApp is a remoting technology, so for each client application that is running, the instance that is running will actually be running on the server. At first glance, this does not seem like a feasible design that can scale well &#8212; or at the very least, cost effectively. Additionally, since this technology is dependent on Remote Desktop, that does imply that a live internet connection is required to use it, which means that if a user doesn&#8217;t have an internet connection, they can&#8217;t use an application used with this. Finally, because of the always-on connectivity requirement, there may be some intensive bandwidth considerations while a user is active with the application.

There are a lot of unknowns with this technology in regards to a ubiquitous .NET client application model, but there are enough intriguing elements here that we thought it merit listing here from an awareness perspective. There are definitely unique &#8212; and innovative &#8212; qualities to appreciate about this clever new offering from the Azure group, and they are worth learning and exploring.

### Noesis GUI Engine

<div class="icon-container">
  <a class="w-inline-block qualityicon cross-platform-icon green" href="/2015/10/ubiquitous-qualities/#native-cross-platform-capable" target="_blank" data-ix="cross-platform-hover"> 
  
  <div class="cross-platform">
    <div class="overlay-container green">
      <div class="overlay-text">
        NATIVE <br />CROSS-PLATFORM <br />CAPABLE
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon html5-icon red" href="/2015/10/ubiquitous-qualities/#html5-compliant" target="_blank" data-ix="html5-hover"> 
  
  <div class="html5-compliant">
    <div class="overlay-container red">
      <div class="overlay-text">
        HTML5 <br />COMPLIANT
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon ux-icon green" href="/2015/10/ubiquitous-qualities/#consistent-user-experience" target="_blank" data-ix="ux-hover"> 
  
  <div class="consistent-ux">
    <div class="overlay-container green">
      <div class="overlay-text">
        CONSISTENT <br />USER <br />EXPERIENCE
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon cross-boundary-icon green" href="/2015/10/ubiquitous-qualities/#cross-boundary-accessibility" target="_blank" data-ix="cross-boundary-hover"> 
  
  <div class="cross-boundary">
    <div class="overlay-container green">
      <div class="overlay-text">
        CROSS-BOUNDARY <br />Accessibility
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon xaml-icon green" href="/2015/10/ubiquitous-qualities/#xaml-powered" target="_blank" data-ix="xaml-hover"> 
  
  <div class="xaml-driven">
    <div class="overlay-container green">
      <div class="overlay-text">
        XAML-POWERED
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon object-congruence-icon green" href="/2015/10/ubiquitous-qualities/#object-serialization-congruence" target="_blank" data-ix="congruence-hover"> 
  
  <div class="object-congruence">
    <div class="overlay-container green">
      <div class="overlay-text">
        OBJECT <br />SERIALIZATION <br />CONGRUENCE
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon holistic-dev-icon green" href="/2015/10/ubiquitous-qualities/#holistic-development-consistency" target="_blank" data-ix="holistic-dev-hover"> 
  
  <div class="holistic-dev">
    <div class="overlay-container green">
      <div class="overlay-text">
        HOLISTIC <br />DEVELOPMENT <br />CONSISTENCY
      </div>
    </div>
  </div></a>
</div>

If I were to build a .NET application right this instant, which tech would I use?  I would use the [Noesis GUI engine][5].  Built primarily for gaming, the Noesis GUI engine is a layer that sits between your 3D scene and your user, providing all the user experience magic that is necessary to make your application awesome.  I&#8217;ve spent some time on the boards there, and I am impressed with this crew.  They care about Xaml and show a lot of passion for their product, something upon which the UWP group could use some study.  In fact, I would consider this the &#8220;real&#8221; UWP as it is a C++ backend at its core, with a C# wrapper.  It was built for gaming but you can use it in any scenario.  However, they are very agile in their approach, and didn&#8217;t take seven years to get markup extensions into their tech.  They are very engaging with their customers and you get the sense they care.  This paired along with a superior understanding of Xaml is why I consider them the de-facto tech for building a .NET application ATM.

### OmniGUI

<div class="icon-container">
  <a class="w-inline-block qualityicon cross-platform-icon green" href="/2015/10/ubiquitous-qualities/#native-cross-platform-capable" target="_blank" data-ix="cross-platform-hover"> 
  
  <div class="cross-platform">
    <div class="overlay-container green">
      <div class="overlay-text">
        NATIVE <br />CROSS-PLATFORM <br />CAPABLE
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon html5-icon red" href="/2015/10/ubiquitous-qualities/#html5-compliant" target="_blank" data-ix="html5-hover"> 
  
  <div class="html5-compliant">
    <div class="overlay-container red">
      <div class="overlay-text">
        HTML5 <br />COMPLIANT
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon ux-icon green" href="/2015/10/ubiquitous-qualities/#consistent-user-experience" target="_blank" data-ix="ux-hover"> 
  
  <div class="consistent-ux">
    <div class="overlay-container green">
      <div class="overlay-text">
        CONSISTENT <br />USER <br />EXPERIENCE
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon cross-boundary-icon green" href="/2015/10/ubiquitous-qualities/#cross-boundary-accessibility" target="_blank" data-ix="cross-boundary-hover"> 
  
  <div class="cross-boundary">
    <div class="overlay-container green">
      <div class="overlay-text">
        CROSS-BOUNDARY <br />Accessibility
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon xaml-icon green" href="/2015/10/ubiquitous-qualities/#xaml-powered" target="_blank" data-ix="xaml-hover"> 
  
  <div class="xaml-driven">
    <div class="overlay-container green">
      <div class="overlay-text">
        XAML-POWERED
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon object-congruence-icon green" href="/2015/10/ubiquitous-qualities/#object-serialization-congruence" target="_blank" data-ix="congruence-hover"> 
  
  <div class="object-congruence">
    <div class="overlay-container green">
      <div class="overlay-text">
        OBJECT <br />SERIALIZATION <br />CONGRUENCE
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon holistic-dev-icon green" href="/2015/10/ubiquitous-qualities/#holistic-development-consistency" target="_blank" data-ix="holistic-dev-hover"> 
  
  <div class="holistic-dev">
    <div class="overlay-container green">
      <div class="overlay-text">
        HOLISTIC <br />DEVELOPMENT <br />CONSISTENCY
      </div>
    </div>
  </div></a>
</div>

From the owner of [OmniXaml][6] springs forth his latest creation, [OmniGUI][7]!  This already looks like it is off to an impressive start.  From the looks of the ReadMe, it has everything we&#8217;re looking for in a ubiquitous client model with the exception of the web support.  However, the big news in this front is that [Mono has been confirmed as being ported over to WebAssembly][8].  Once that is complete, we will be able to use the Mono .NET runtime within a WebAssembly environment, which would mean running .NET within a browser, once again!

SuperJMN, the creator of OmniXaml and OmniGUI has a solid head on his shoulders and it is good to see the work he is doing in this area.  It is as if he is doing the work of an entire MSFT division all by himself.  And considering that he understands ubiquity better than the entire UWP group, the case could be made that he is doing exactly that.  He truly is Super!  For more information and details around OmniGUI, feel free to check out the [discussion I started here][9].

## Web-Hosted Client Application Models

All of the listed .NET client application models described so far have been &#8220;native&#8221; or &#8220;compiled&#8221; or &#8220;store-hosted&#8221; in nature. Now we start to move into client application models that run primarily in the context of a HTML5 runtime instance, or browser.

### ASP.NET-Hosted (HTML5) Client Application

<div class="icon-container">
  <a class="w-inline-block qualityicon cross-platform-icon red" href="/2015/10/ubiquitous-qualities/#native-cross-platform-capable" target="_blank" data-ix="cross-platform-hover"> 
  
  <div class="cross-platform">
    <div class="overlay-container red">
      <div class="overlay-text">
        NATIVE <br />CROSS-PLATFORM <br />CAPABLE
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon html5-icon green" href="/2015/10/ubiquitous-qualities/#html5-compliant" target="_blank" data-ix="html5-hover"> 
  
  <div class="html5-compliant">
    <div class="overlay-container green">
      <div class="overlay-text">
        HTML5 <br />COMPLIANT
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon ux-icon green" href="/2015/10/ubiquitous-qualities/#consistent-user-experience" target="_blank" data-ix="ux-hover"> 
  
  <div class="consistent-ux">
    <div class="overlay-container green">
      <div class="overlay-text">
        CONSISTENT <br />USER <br />EXPERIENCE
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon cross-boundary-icon red" href="/2015/10/ubiquitous-qualities/#cross-boundary-accessibility" target="_blank" data-ix="cross-boundary-hover"> 
  
  <div class="cross-boundary">
    <div class="overlay-container red">
      <div class="overlay-text">
        CROSS-BOUNDARY <br />Accessibility
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon xaml-icon red" href="/2015/10/ubiquitous-qualities/#xaml-powered" target="_blank" data-ix="xaml-hover"> 
  
  <div class="xaml-driven">
    <div class="overlay-container red">
      <div class="overlay-text">
        XAML-POWERED
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon object-congruence-icon red" href="/2015/10/ubiquitous-qualities/#object-serialization-congruence" target="_blank" data-ix="congruence-hover"> 
  
  <div class="object-congruence">
    <div class="overlay-container red">
      <div class="overlay-text">
        OBJECT <br />SERIALIZATION <br />CONGRUENCE
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon holistic-dev-icon green" href="/2015/10/ubiquitous-qualities/#holistic-development-consistency" target="_blank" data-ix="holistic-dev-hover"> 
  
  <div class="holistic-dev">
    <div class="overlay-container green">
      <div class="overlay-text">
        HOLISTIC <br />DEVELOPMENT <br />CONSISTENCY
      </div>
    </div>
  </div></a>
</div> Our first model is actually a hybrid of these two contexts, and it is the model found in 

<a href="https://asp.net" target="_blank" rel="noopener">ASP.NET</a> applications. This model is hosted and executed on the server in its own boundary, and can live in the same tier or different tier than the primary application services in which it communicates. When a page is requested and processed from the server, it is created by ASP.NET and ultimately emits HTML5 and JavaScript, and sends the results to the requesting client.</p> 

Here, we start to encounter and understand the challenges associated with web application client models. The emitted HTML5 and JavaScript in no way is connected with the .NET artifacts that execute on the server. Therefore, state that does not require server interaction must be maintained on the client through means of HTML5 element interaction and JavaScript. The use of this state (and application) management in JavaScript on the client, along with .NET on the server violates the requirement of cross-boundary capable artifacts. Additionally, the requirement for consistent development guidelines to define these objects is also violated as prescribed JavaScript naming conventions and guidelines are completely different from .NET&#8217;s. Finally, ASP.NET primarily describes its objects through a syntax known as Razor, and does not satisfy our requirement for a Xaml-driven description model.

Nonetheless, it is conceivably possible to think of ASP.NET in the near future as a possible cross-platform (albeit not ubiquitous) .NET client application model. That is, by hosting a ASP.NET server process in a Droid and/or iOS application process, ASP.NET could satisfy the cross-platform capability requirement by essentially running a server in a cross-platform context and serve up pages through a web-view control on the native device. More thoughts around this intriguing possibility <a href="http://forums.dotnetfoundation.org/t/crazy-idea-run-asp-net5-on-android/1074" target="_blank" rel="noopener">can be found here</a>.

### HTML5

<div class="icon-container">
  <a class="w-inline-block qualityicon cross-platform-icon red" href="/2015/10/ubiquitous-qualities/#native-cross-platform-capable" target="_blank" data-ix="cross-platform-hover"> 
  
  <div class="cross-platform">
    <div class="overlay-container red">
      <div class="overlay-text">
        NATIVE <br />CROSS-PLATFORM <br />CAPABLE
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon html5-icon green" href="/2015/10/ubiquitous-qualities/#html5-compliant" target="_blank" data-ix="html5-hover"> 
  
  <div class="html5-compliant">
    <div class="overlay-container green">
      <div class="overlay-text">
        HTML5 <br />COMPLIANT
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon ux-icon green" href="/2015/10/ubiquitous-qualities/#consistent-user-experience" target="_blank" data-ix="ux-hover"> 
  
  <div class="consistent-ux">
    <div class="overlay-container green">
      <div class="overlay-text">
        CONSISTENT <br />USER <br />EXPERIENCE
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon cross-boundary-icon red" href="/2015/10/ubiquitous-qualities/#cross-boundary-accessibility" target="_blank" data-ix="cross-boundary-hover"> 
  
  <div class="cross-boundary">
    <div class="overlay-container red">
      <div class="overlay-text">
        CROSS-BOUNDARY <br />Accessibility
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon xaml-icon red" href="/2015/10/ubiquitous-qualities/#xaml-powered" target="_blank" data-ix="xaml-hover"> 
  
  <div class="xaml-driven">
    <div class="overlay-container red">
      <div class="overlay-text">
        XAML-POWERED
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon object-congruence-icon red" href="/2015/10/ubiquitous-qualities/#object-serialization-congruence" target="_blank" data-ix="congruence-hover"> 
  
  <div class="object-congruence">
    <div class="overlay-container red">
      <div class="overlay-text">
        OBJECT <br />SERIALIZATION <br />CONGRUENCE
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon holistic-dev-icon red" href="/2015/10/ubiquitous-qualities/#holistic-development-consistency" target="_blank" data-ix="holistic-dev-hover"> 
  
  <div class="holistic-dev">
    <div class="overlay-container red">
      <div class="overlay-text">
        HOLISTIC <br />DEVELOPMENT <br />CONSISTENCY
      </div>
    </div>
  </div></a>
</div> The 

<a href="https://en.wikipedia.org/wiki/HTML5" target="_blank" rel="noopener">HTML5</a> client application model can currently be viewed as the oil to .NET&#8217;s water. In seemingly every aspect, from markup language to interpreted language, the HTML5 client application development experience is unlike any counterpart found in a .NET client application model. However, the HTML5 standard is an established, embraced, and popular standard since October 2014. By abiding and following this standard, it has accomplished a goal that .NET has failed to do to this day: ubiquity. Every HTML5 application written to its standard has a very high probability (<a href="https://html5test.com/" target="_blank" rel="noopener">minor differences do exist</a>) that it will run and operate exactly the same no matter the browser or OS used to view the application. This not only satisfies our requirement for a consistent user experience, but makes HTML5 a truly ubiquitous client application model, and one in which we are basing our goal here for a ubiquitous **.NET** client application model.</p> 

An HTML5 application is written in HTML5-compliant HTML, and JavaScript as the interpreted language of choice. Both of these offerings are incompatible with .NET models and architecture. Because of this, there is no Xaml, or .NET, .NET Development Guidelines, or shared code between application boundaries. In fact, if you have a component written in .NET on the server, you must write its equivalent in JavaScript (or <a href="http://www.typescriptlang.org/" target="_blank" rel="noopener">TypeScript</a>) for the client.

Oil and water, indeed.

This is a very expensive and complicated problem, and it is any wonder why the Visual Studio team has <a href="http://visualstudio.uservoice.com/forums/121579-visual-studio/suggestions/3556619-silverlight-6" target="_blank" rel="noopener">inexplicably guided 16,000 voting users of Silverlight to build their applications using HTML5</a> instead, when doing so will incur twice the code since sharing code between client and server is no longer possible in an HTML5 client application model as it was in Silverlight. In a future post of this series, we will discuss this problem more at length.

### CSHTML5

<div class="icon-container">
  <a class="w-inline-block qualityicon cross-platform-icon red" href="/2015/10/ubiquitous-qualities/#native-cross-platform-capable" target="_blank" data-ix="cross-platform-hover"> 
  
  <div class="cross-platform">
    <div class="overlay-container red">
      <div class="overlay-text">
        NATIVE <br />CROSS-PLATFORM <br />CAPABLE
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon html5-icon green" href="/2015/10/ubiquitous-qualities/#html5-compliant" target="_blank" data-ix="html5-hover"> 
  
  <div class="html5-compliant">
    <div class="overlay-container green">
      <div class="overlay-text">
        HTML5 <br />COMPLIANT
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon ux-icon green" href="/2015/10/ubiquitous-qualities/#consistent-user-experience" target="_blank" data-ix="ux-hover"> 
  
  <div class="consistent-ux">
    <div class="overlay-container green">
      <div class="overlay-text">
        CONSISTENT <br />USER <br />EXPERIENCE
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon cross-boundary-icon red" href="/2015/10/ubiquitous-qualities/#cross-boundary-accessibility" target="_blank" data-ix="cross-boundary-hover"> 
  
  <div class="cross-boundary">
    <div class="overlay-container red">
      <div class="overlay-text">
        CROSS-BOUNDARY <br />Accessibility
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon xaml-icon green" href="/2015/10/ubiquitous-qualities/#xaml-powered" target="_blank" data-ix="xaml-hover"> 
  
  <div class="xaml-driven">
    <div class="overlay-container green">
      <div class="overlay-text">
        XAML-POWERED
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon object-congruence-icon green" href="/2015/10/ubiquitous-qualities/#object-serialization-congruence" target="_blank" data-ix="congruence-hover"> 
  
  <div class="object-congruence">
    <div class="overlay-container green">
      <div class="overlay-text">
        OBJECT <br />SERIALIZATION <br />CONGRUENCE
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon holistic-dev-icon green" href="/2015/10/ubiquitous-qualities/#holistic-development-consistency" target="_blank" data-ix="holistic-dev-hover"> 
  
  <div class="holistic-dev">
    <div class="overlay-container green">
      <div class="overlay-text">
        HOLISTIC <br />DEVELOPMENT <br />CONSISTENCY
      </div>
    </div>
  </div></a>
</div> From oil, back to life-giving water again. 

<a href="http://cshtml5.com/" target="_blank" rel="noopener">CSHTML5</a> is an amazing project that does not get enough consideration, exposure, or press it seems. It is based off a an even more amazing project known as <a href="http://JSIL.org" target="_blank" rel="noopener">JSIL.org</a>. JSIL.org is a project that takes .NET code and transpiles it into HTML5 and web-standards artifacts. If this sounds like something an entire division at Microsoft should be dedicated to, rather than some wiz-kid out of California, then you are not alone. Here we have a project that accomplishes the seemingly impossible: reconciling the differences between a .NET client application model and an HTML5 client application model. CSHTML5 is based on <a href="http://JSIL.org" target="_blank" rel="noopener">JSIL.org</a> and enables Xaml-defined and described applications to run in any HTML5-compliant browser. With this, you get .NET assemblies, guidelines, and consistency between client and server development.</p> 

Perfection, right?

Well, almost. As great as CSHTML5 is, it does currently suffer from some challenges that we have outlined here:

  * CSHTML5 is currently run by a smaller company and lacks the proper development resources for a truly revolutionary change. Again, we feel this is a problem space that an entire group within Microsoft should be dedicated to solving.
  * While it is possible to &#8220;share&#8221; code between client and server projects (through the use of linked files) in a CSHTML5 solution, you cannot share them in the way as you can in a traditional .NET solution, which is what is expected in our Cross-Boundary Accessibility requirement. Additionally, CSHTML5 does not support Portable Class Libraries at the moment, so that also does not satisfy this requirement.
  * Finally, with CSHTML5 it is possible (or will be possible), to host an application in a cross-platform native web control and gain cross-platform native capability, much like the same way that <a href="https://cordova.apache.org/" target="_blank" rel="noopener">Cordova</a> operates. This appears to meet our requirement for cross-platform native support. However, when we think of cross-platform capability, we mean to see our ubiquitous .NET client application model compile to the target platform&#8217;s native byte-code.
  * Performance is also a present consideration, as you would expect from a beta product.

With all of this said, in our view, _CSHTML5 is at present the closest thing to a ubiquitous .NET client application model in the current marketplace_. However, it does suffer from lack of momentum and resources, as well as key features to make it the perfect and recommended model. It is our wish to see Microsoft partner with CSHTML5/JSIL.org and incorporate this as an official technology in the Microsoft landscape, and leverage it towards building a ubiquitous .NET client application model.

### WebSharper

<div class="icon-container">
  <a class="w-inline-block qualityicon cross-platform-icon red" href="/2015/10/ubiquitous-qualities/#native-cross-platform-capable" target="_blank" data-ix="cross-platform-hover"> 
  
  <div class="cross-platform">
    <div class="overlay-container red">
      <div class="overlay-text">
        NATIVE <br />CROSS-PLATFORM <br />CAPABLE
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon html5-icon green" href="/2015/10/ubiquitous-qualities/#html5-compliant" target="_blank" data-ix="html5-hover"> 
  
  <div class="html5-compliant">
    <div class="overlay-container green">
      <div class="overlay-text">
        HTML5 <br />COMPLIANT
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon ux-icon green" href="/2015/10/ubiquitous-qualities/#consistent-user-experience" target="_blank" data-ix="ux-hover"> 
  
  <div class="consistent-ux">
    <div class="overlay-container green">
      <div class="overlay-text">
        CONSISTENT <br />USER <br />EXPERIENCE
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon cross-boundary-icon green" href="/2015/10/ubiquitous-qualities/#cross-boundary-accessibility" target="_blank" data-ix="cross-boundary-hover"> 
  
  <div class="cross-boundary">
    <div class="overlay-container green">
      <div class="overlay-text">
        CROSS-BOUNDARY <br />Accessibility
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon xaml-icon red" href="/2015/10/ubiquitous-qualities/#xaml-powered" target="_blank" data-ix="xaml-hover"> 
  
  <div class="xaml-driven">
    <div class="overlay-container red">
      <div class="overlay-text">
        XAML-POWERED
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon object-congruence-icon red" href="/2015/10/ubiquitous-qualities/#object-serialization-congruence" target="_blank" data-ix="congruence-hover"> 
  
  <div class="object-congruence">
    <div class="overlay-container red">
      <div class="overlay-text">
        OBJECT <br />SERIALIZATION <br />CONGRUENCE
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon holistic-dev-icon green" href="/2015/10/ubiquitous-qualities/#holistic-development-consistency" target="_blank" data-ix="holistic-dev-hover"> 
  
  <div class="holistic-dev">
    <div class="overlay-container green">
      <div class="overlay-text">
        HOLISTIC <br />DEVELOPMENT <br />CONSISTENCY
      </div>
    </div>
  </div></a>
</div>

<a href="http://www.websharper.com/" target="_blank" rel="noopener">WebSharper</a> is a promising web-hosted client application model that features F#-to-JavaScript transpilation. <a href="http://intellifactory.com/" target="_blank" rel="noopener">IntelliFactory</a>, the company behind this model, is hard at work making additional features that will be available soon in alpha releases, the most notable of these being C# support. WebSharper works by creating a model around the HTML5 DOM. It uses a templating system around HTML5 files, so Xaml is not utilized in any way. Code is written in F# (.NET) and which is ultimately injected into the HTML5 DOM where traditional JavaScript APIs such as Bootstrap and jQuery can take over and work with those elements. Additionally, you can use code between client and server, so that does appear to satisfy cross-boundary accessibility, at least for F#. We will have to wait for C# support to know for certain if it fully satisfies all use cases. For instance, Portable Class Library-support is not available yet but that is slated as a future feature.  
As WebSharper doesn&#8217;t offer native-compiled support, or Xaml support, and works with the HTML5 DOM as its client model, it lacks all the requirements for what we are looking for in a ubiquitous .NET client application development model offering. Nonetheless, with all of its interesting current and planned features, it is one to keep an eye on as new versions are released.

### DuoCo.de

<div class="icon-container">
  <a class="w-inline-block qualityicon cross-platform-icon red" href="/2015/10/ubiquitous-qualities/#native-cross-platform-capable" target="_blank" data-ix="cross-platform-hover"> 
  
  <div class="cross-platform">
    <div class="overlay-container red">
      <div class="overlay-text">
        NATIVE <br />CROSS-PLATFORM <br />CAPABLE
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon html5-icon green" href="/2015/10/ubiquitous-qualities/#html5-compliant" target="_blank" data-ix="html5-hover"> 
  
  <div class="html5-compliant">
    <div class="overlay-container green">
      <div class="overlay-text">
        HTML5 <br />COMPLIANT
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon ux-icon green" href="/2015/10/ubiquitous-qualities/#consistent-user-experience" target="_blank" data-ix="ux-hover"> 
  
  <div class="consistent-ux">
    <div class="overlay-container green">
      <div class="overlay-text">
        CONSISTENT <br />USER <br />EXPERIENCE
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon cross-boundary-icon red" href="/2015/10/ubiquitous-qualities/#cross-boundary-accessibility" target="_blank" data-ix="cross-boundary-hover"> 
  
  <div class="cross-boundary">
    <div class="overlay-container red">
      <div class="overlay-text">
        CROSS-BOUNDARY <br />Accessibility
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon xaml-icon red" href="/2015/10/ubiquitous-qualities/#xaml-powered" target="_blank" data-ix="xaml-hover"> 
  
  <div class="xaml-driven">
    <div class="overlay-container red">
      <div class="overlay-text">
        XAML-POWERED
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon object-congruence-icon red" href="/2015/10/ubiquitous-qualities/#object-serialization-congruence" target="_blank" data-ix="congruence-hover"> 
  
  <div class="object-congruence">
    <div class="overlay-container red">
      <div class="overlay-text">
        OBJECT <br />SERIALIZATION <br />CONGRUENCE
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon holistic-dev-icon green" href="/2015/10/ubiquitous-qualities/#holistic-development-consistency" target="_blank" data-ix="holistic-dev-hover"> 
  
  <div class="holistic-dev">
    <div class="overlay-container green">
      <div class="overlay-text">
        HOLISTIC <br />DEVELOPMENT <br />CONSISTENCY
      </div>
    </div>
  </div></a>
</div>

Another JavaScript transpiler technology, <a href="http://duoco.de" target="_blank" rel="noopener">DuoCo.de</a> enables you to transpile your C#/VB.NET projects into HTML5-compliant artifacts. Duoco.de takes a more efficient transpilation route than JSIL in that it uses Roslyn to generate the JavaScript. However, the client model philosophy of DuoCo.de is different than CSHTML5. While it does provide the ability to transpile C#/VB.NET artifacts into JavaScript, DuoCo.de is designed to operate in the context of an HTML5 client application model. This means using HTML5 elements and markup to describe your application, rather than a Xaml-driven approach. This is an incongruous approach and one that does not align with our requirements or vision of a ubiquitous .NET client application model. Additionally, since Duoco.de transpiles via Roslyn, it only (currently) supports the languages that Roslyn supports, which at present is C# and VB.NET. This leaves other important languages like F# (even though _every_ .NET language is important!) out of the realm of possibility to use with Duoco.de.

### Bridge.NET

<div class="icon-container">
  <a class="w-inline-block qualityicon cross-platform-icon red" href="/2015/10/ubiquitous-qualities/#native-cross-platform-capable" target="_blank" data-ix="cross-platform-hover"> 
  
  <div class="cross-platform">
    <div class="overlay-container red">
      <div class="overlay-text">
        NATIVE <br />CROSS-PLATFORM <br />CAPABLE
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon html5-icon green" href="/2015/10/ubiquitous-qualities/#html5-compliant" target="_blank" data-ix="html5-hover"> 
  
  <div class="html5-compliant">
    <div class="overlay-container green">
      <div class="overlay-text">
        HTML5 <br />COMPLIANT
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon ux-icon green" href="/2015/10/ubiquitous-qualities/#consistent-user-experience" target="_blank" data-ix="ux-hover"> 
  
  <div class="consistent-ux">
    <div class="overlay-container green">
      <div class="overlay-text">
        CONSISTENT <br />USER <br />EXPERIENCE
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon cross-boundary-icon red" href="/2015/10/ubiquitous-qualities/#cross-boundary-accessibility" target="_blank" data-ix="cross-boundary-hover"> 
  
  <div class="cross-boundary">
    <div class="overlay-container red">
      <div class="overlay-text">
        CROSS-BOUNDARY <br />Accessibility
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon xaml-icon red" href="/2015/10/ubiquitous-qualities/#xaml-powered" target="_blank" data-ix="xaml-hover"> 
  
  <div class="xaml-driven">
    <div class="overlay-container red">
      <div class="overlay-text">
        XAML-POWERED
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon object-congruence-icon red" href="/2015/10/ubiquitous-qualities/#object-serialization-congruence" target="_blank" data-ix="congruence-hover"> 
  
  <div class="object-congruence">
    <div class="overlay-container red">
      <div class="overlay-text">
        OBJECT <br />SERIALIZATION <br />CONGRUENCE
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon holistic-dev-icon green" href="/2015/10/ubiquitous-qualities/#holistic-development-consistency" target="_blank" data-ix="holistic-dev-hover"> 
  
  <div class="holistic-dev">
    <div class="overlay-container green">
      <div class="overlay-text">
        HOLISTIC <br />DEVELOPMENT <br />CONSISTENCY
      </div>
    </div>
  </div></a>
</div>

Like Duoco.de, <a href="http://Bridge.NET" target="_blank" rel="noopener">Bridge.NET</a> is another C#-to-JavaScript compiler that allows you to work in the HTML5 client application model paradigm.  They have built C# APIs around the major JavaScript-based equivalents and the expectation is to operate within the context of an HTML5 page, complete with DOM and related elements.  So Xaml is not a supported mechanism in this model as of today.  Bridge.NET is also similar to Duoco.de in that it is tied into Roslyn for all of its magic.  However, unlike Duoco.de, Bridge.NET is <a href="https://github.com/bridgedotnet/" target="_blank" rel="noopener">open-source</a> and appears to have a healthy community around it.  Like all the other .NET-to-JavaScript transpilers in the present market, Bridge.NET <a href="https://github.com/bridgedotnet/Bridge/issues/695" target="_blank" rel="noopener">does not enable portable class library support at the moment</a>, so the holy grail of <a href="/2015/10/ubiquitous-qualities/#cross-boundary-accessibility" target="_blank" rel="noopener">Cross-Boundary Accessibility</a> remains illusive.   All said, I will say that of all the products in this area that I have seen to date, Bridge.NET looks the most professional and promising.  It will be interesting to watch their progress (closely!) to see if they manage to get PCL support, and maybe leverage their great professional look to even partnership with Microsoft to help enable integration with its new cross-platform initiatives.

###  Fayde

<div class="icon-container">
  <a class="w-inline-block qualityicon cross-platform-icon red" href="/2015/10/ubiquitous-qualities/#native-cross-platform-capable" target="_blank" data-ix="cross-platform-hover"> 
  
  <div class="cross-platform">
    <div class="overlay-container red">
      <div class="overlay-text">
        NATIVE <br />CROSS-PLATFORM <br />CAPABLE
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon html5-icon green" href="/2015/10/ubiquitous-qualities/#html5-compliant" target="_blank" data-ix="html5-hover"> 
  
  <div class="html5-compliant">
    <div class="overlay-container green">
      <div class="overlay-text">
        HTML5 <br />COMPLIANT
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon ux-icon green" href="/2015/10/ubiquitous-qualities/#consistent-user-experience" target="_blank" data-ix="ux-hover"> 
  
  <div class="consistent-ux">
    <div class="overlay-container green">
      <div class="overlay-text">
        CONSISTENT <br />USER <br />EXPERIENCE
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon cross-boundary-icon red" href="/2015/10/ubiquitous-qualities/#cross-boundary-accessibility" target="_blank" data-ix="cross-boundary-hover"> 
  
  <div class="cross-boundary">
    <div class="overlay-container red">
      <div class="overlay-text">
        CROSS-BOUNDARY <br />Accessibility
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon xaml-icon green" href="/2015/10/ubiquitous-qualities/#xaml-powered" target="_blank" data-ix="xaml-hover"> 
  
  <div class="xaml-driven">
    <div class="overlay-container green">
      <div class="overlay-text">
        XAML-POWERED
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon object-congruence-icon green" href="/2015/10/ubiquitous-qualities/#object-serialization-congruence" target="_blank" data-ix="congruence-hover"> 
  
  <div class="object-congruence">
    <div class="overlay-container green">
      <div class="overlay-text">
        OBJECT <br />SERIALIZATION <br />CONGRUENCE
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon holistic-dev-icon red" href="/2015/10/ubiquitous-qualities/#holistic-development-consistency" target="_blank" data-ix="holistic-dev-hover"> 
  
  <div class="holistic-dev">
    <div class="overlay-container red">
      <div class="overlay-text">
        HOLISTIC <br />DEVELOPMENT <br />CONSISTENCY
      </div>
    </div>
  </div></a>
</div>

Next, we wanted to mention <a href="http://wsick.github.io/Fayde/" target="_blank" rel="noopener">Fayde</a>, another creative client application model that has <a href="http://www.hanselman.com/blog/JavaScriptHasWonRunFlashWithMozillaShumwayAndDevelopSilverlightInJSWithFayde.aspx" target="_blank" rel="noopener">gotten some acclaim</a>. Fayde does have some strong Silverlight-based roots, is Xaml-driven, and bases its outputs in performant web-based artifacts. While Fayde is Xaml-driven, its code is expected to be developed in TypeScript/JavaScript. This breaks our requirement for a cross-boundary accessibility.

### Blazor

<div class="icon-container">
  <a class="w-inline-block qualityicon cross-platform-icon red" href="/2015/10/ubiquitous-qualities/#native-cross-platform-capable" target="_blank" data-ix="cross-platform-hover"> 
  
  <div class="cross-platform">
    <div class="overlay-container red">
      <div class="overlay-text">
        NATIVE <br />CROSS-PLATFORM <br />CAPABLE
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon html5-icon green" href="/2015/10/ubiquitous-qualities/#html5-compliant" target="_blank" data-ix="html5-hover"> 
  
  <div class="html5-compliant">
    <div class="overlay-container green">
      <div class="overlay-text">
        HTML5 <br />COMPLIANT
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon ux-icon green" href="/2015/10/ubiquitous-qualities/#consistent-user-experience" target="_blank" data-ix="ux-hover"> 
  
  <div class="consistent-ux">
    <div class="overlay-container green">
      <div class="overlay-text">
        CONSISTENT <br />USER <br />EXPERIENCE
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon cross-boundary-icon green" href="/2015/10/ubiquitous-qualities/#cross-boundary-accessibility" target="_blank" data-ix="cross-boundary-hover"> 
  
  <div class="cross-boundary">
    <div class="overlay-container green">
      <div class="overlay-text">
        CROSS-BOUNDARY <br />Accessibility
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon xaml-icon red" href="/2015/10/ubiquitous-qualities/#xaml-powered" target="_blank" data-ix="xaml-hover"> 
  
  <div class="xaml-driven">
    <div class="overlay-container red">
      <div class="overlay-text">
        XAML-POWERED
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon object-congruence-icon red" href="/2015/10/ubiquitous-qualities/#object-serialization-congruence" target="_blank" data-ix="congruence-hover"> 
  
  <div class="object-congruence">
    <div class="overlay-container red">
      <div class="overlay-text">
        OBJECT <br />SERIALIZATION <br />CONGRUENCE
      </div>
    </div>
  </div></a> 
  
  <a class="w-inline-block qualityicon holistic-dev-icon green" href="/2015/10/ubiquitous-qualities/#holistic-development-consistency" target="_blank" data-ix="holistic-dev-hover"> 
  
  <div class="holistic-dev">
    <div class="overlay-container green">
      <div class="overlay-text">
        HOLISTIC <br />DEVELOPMENT <br />CONSISTENCY
      </div>
    </div>
  </div></a>
</div>

This entry was brought to our attention by Scott &#8220;The Man&#8221; Hanselman himself. [Blazor][10] is an &#8220;unofficial&#8221; Microsoft entry into WebAssembly, which is a promising and encouraging endeavor by the software giant. This is currently a side project but you can immediately see that it has potential to quickly evolve into its own franchise. If Microsoft was smart it would indeed do this and promote the venerable Steve Sanderson immediately to a full-time guardian of this project.

While this project is a great step forward for Microsoft client models in that it finally hosts a .NET client model in the web browser process, it does fall short in our list of requirements for a ubiquitous .NET client development model. First, it does use HTML5 as its client view system. While this does promote our [consistent UX requirement][11], it does break from our desire for [object serialization congruence][12] between view markup and rendered objects in memory (e.g. using a `p` tag to notate a container as opposed to a `StackPanel` or `DockPanel`).

Further, as Blazor is meant to be more of an introductory project into WebAssembly, it does not at moment support any sort of native scenarios. That does not mean of course that given enough time and resources (as, again, MSFT should do) that this is not possible. But at the moment you would be required to build two view bases to support all known platforms, adding to the overall costs of the solution. It would be great to see this somehow render in a native scenario, thereby reducing required code and views. If it can be done in Xaml, all the better.

### Summary Matrix

To summarize all models with the desired qualities, we have created the following grid to cross-reference all known client application models with our desired qualities for a ubiquitous .NET client application development model.

<table id="cross-reference" class="chart" cellspacing="0">
  <caption> 
  
  <h4>
    Capability Matrix for .NET Client Application Models
  </h4></caption> 
  
  <tr>
    <th>
      &nbsp;
    </th>
    
    <th>
      <a class="w-inline-block qualityicon cross-platform-icon" href="/2015/10/ubiquitous-qualities/#native-cross-platform-capable" target="_blank" data-ix="cross-platform-hover"> 
      
      <div class="cross-platform">
        <div class="overlay-container">
          <div class="overlay-text">
            Native Cross-Platform Capable
          </div>
        </div>
      </div></a>
    </th>
    
    <th>
      <a class="w-inline-block qualityicon html5-icon" href="/2015/10/ubiquitous-qualities/#html5-compliant" target="_blank" data-ix="html5-hover"> 
      
      <div class="html5-compliant">
        <div class="overlay-container">
          <div class="overlay-text">
            HTML5-Compliant
          </div>
        </div>
      </div></a>
    </th>
    
    <th>
      <a class="w-inline-block qualityicon ux-icon" href="/2015/10/ubiquitous-qualities/#consistent-user-experience" target="_blank" data-ix="ux-hover"> 
      
      <div class="consistent-ux">
        <div class="overlay-container">
          <div class="overlay-text">
            Consistent UX
          </div>
        </div>
      </div></a>
    </th>
    
    <th>
      <a class="w-inline-block qualityicon cross-boundary-icon" href="/2015/10/ubiquitous-qualities/#cross-boundary-accessibility" target="_blank" data-ix="cross-boundary-hover"> 
      
      <div class="cross-boundary">
        <div class="overlay-container">
          <div class="overlay-text">
            Cross-Boundary Accessibility
          </div>
        </div>
      </div></a>
    </th>
    
    <th>
      <a class="w-inline-block qualityicon xaml-icon" href="/2015/10/ubiquitous-qualities/#xaml-powered" target="_blank" data-ix="xaml-hover"> 
      
      <div class="xaml-driven">
        <div class="overlay-container">
          <div class="overlay-text">
            XAML-Powered
          </div>
        </div>
      </div></a>
    </th>
    
    <th>
      <a class="w-inline-block qualityicon object-congruence-icon" href="/2015/10/ubiquitous-qualities/#object-serialization-congruence" target="_blank" data-ix="congruence-hover"> 
      
      <div class="object-congruence">
        <div class="overlay-container">
          <div class="overlay-text">
            Object Serialization Congruence
          </div>
        </div>
      </div></a>
    </th>
    
    <th>
      <a class="w-inline-block qualityicon holistic-dev-icon" href="/2015/10/ubiquitous-qualities/#holistic-development-consistency" target="_blank" data-ix="holistic-dev-hover"> 
      
      <div class="holistic-dev">
        <div class="overlay-container">
          <div class="overlay-text">
            Holistic Development Consistency
          </div>
        </div>
      </div></a>
    </th>
  </tr>
  
  <tr>
    <th title="Click to view more details.">
      <h5>
        <a href="#windows-forms">Windows Forms</a>
      </h5>
    </th>
    
    <td class="no">
      <i class="icon"></i>
    </td>
    
    <td class="no">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
    
    <td class="no">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
  </tr>
  
  <tr>
    <th title="Click to view more details.">
      <h5>
        <a href="#windows-presentation-foundation">Windows Presentation Foundation</a>
      </h5>
    </th>
    
    <td class="no">
      <i class="icon"></i>
    </td>
    
    <td class="no">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
  </tr>
  
  <tr>
    <th title="Click to view more details.">
      <h5>
        <a href="#silverlight">Silverlight</a>
      </h5>
    </th>
    
    <td class="no">
      <i class="icon"></i>
    </td>
    
    <td class="no">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
  </tr>
  
  <tr>
    <th title="Click to view more details.">
      <h5>
        <a href="#universal-windows-platform">Universal Windows Platform</a>
      </h5>
    </th>
    
    <td class="no">
      <i class="icon"></i>
    </td>
    
    <td class="no">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
    
    <td class="no">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
  </tr>
  
  <tr>
    <th title="Click to view more details.">
      <h5>
        <a href="#xamarinforms">Xamarin.Forms</a>
      </h5>
    </th>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
    
    <td class="no">
      <i class="icon"></i>
    </td>
    
    <td class="no">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
  </tr>
  
  <tr>
    <th title="Click to view more details.">
      <h5>
        <a href="#avalonia">Avalonia</a>
      </h5>
    </th>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
    
    <td class="no">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
  </tr>
  
  <tr>
    <th title="Click to view more details.">
      <h5>
        <a href="#urho3d">Urho3D</a>
      </h5>
    </th>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
    
    <td class="no">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
    
    <td class="no">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
  </tr>
  
  <tr>
    <th title="Click to view more details.">
      <h5>
        <a href="#x2h-xaml-to-html-translator">xaml2html</a>
      </h5>
    </th>
    
    <td class="no">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
    
    <td class="no">
      <i class="icon"></i>
    </td>
    
    <td class="no">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
  </tr>
  
  <tr>
    <th title="Click to view more details.">
      <h5>
        <a href="#azure-powerapps">Azure PowerApps</a>
      </h5>
    </th>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
    
    <td class="no">
      <i class="icon"></i>
    </td>
    
    <td class="no">
      <i class="icon"></i>
    </td>
    
    <td class="no">
      <i class="icon"></i>
    </td>
    
    <td class="no">
      <i class="icon"></i>
    </td>
  </tr>
  
  <tr>
    <th title="Click to view more details.">
      <h5>
        <a href="#azure-remoteapp">Azure RemoteApp</a>
      </h5>
    </th>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
    
    <td class="no">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
  </tr>
  
  <tr>
    <th title="Click to view more details.">
      <h5>
        <a href="#noesis-gui-engine">Noesis GUI Engine</a>
      </h5>
    </th>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
    
    <td class="no">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
  </tr>
  
  <tr>
    <th title="Click to view more details.">
      <h5>
        <a href="#omnigui">OmniGUI</a>
      </h5>
    </th>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
    
    <td class="no">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
  </tr>
  
  <tr>
    <th title="Click to view more details.">
      <h5>
        <a href="#aspnet-hosted-html5-client-application">ASP.NET-Hosted (HTML5) Client Application</a>
      </h5>
    </th>
    
    <td class="no">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
    
    <td class="no">
      <i class="icon"></i>
    </td>
    
    <td class="no">
      <i class="icon"></i>
    </td>
    
    <td class="no">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
  </tr>
  
  <tr>
    <th title="Click to view more details.">
      <h5>
        <a href="#html5">HTML5</a>
      </h5>
    </th>
    
    <td class="no">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
    
    <td class="no">
      <i class="icon"></i>
    </td>
    
    <td class="no">
      <i class="icon"></i>
    </td>
    
    <td class="no">
      <i class="icon"></i>
    </td>
    
    <td class="no">
      <i class="icon"></i>
    </td>
  </tr>
  
  <tr>
    <th title="Click to view more details.">
      <h5>
        <a href="#cshtml5">CSHTML5</a>
      </h5>
    </th>
    
    <td class="no">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
    
    <td class="no">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
  </tr>
  
  <tr>
    <th title="Click to view more details.">
      <h5>
        <a href="#websharper">WebSharper</a>
      </h5>
    </th>
    
    <td class="no">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
    
    <td class="no">
      <i class="icon"></i>
    </td>
    
    <td class="no">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
  </tr>
  
  <tr>
    <th title="Click to view more details.">
      <h5>
        <a href="#duocode">Duoco.de</a>
      </h5>
    </th>
    
    <td class="no">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
    
    <td class="no">
      <i class="icon"></i>
    </td>
    
    <td class="no">
      <i class="icon"></i>
    </td>
    
    <td class="no">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
  </tr>
  
  <tr>
    <th title="Click to view more details.">
      <h5>
        <a href="#bridgenet">Bridge.NET</a>
      </h5>
    </th>
    
    <td class="no">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
    
    <td class="no">
      <i class="icon"></i>
    </td>
    
    <td class="no">
      <i class="icon"></i>
    </td>
    
    <td class="no">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
  </tr>
  
  <tr>
    <th title="Click to view more details.">
      <h5>
        <a href="#fayde">Fayde</a>
      </h5>
    </th>
    
    <td class="no">
      <i class="icon"></i>
    </td>
    
    <td class="no">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
    
    <td class="no">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
    
    <td class="no">
      <i class="icon"></i>
    </td>
  </tr>
  
  <tr>
    <th title="Click to view more details.">
      <h5>
        <a href="#blazor">Blazor</a>
      </h5>
    </th>
    
    <td class="no">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
    
    <td class="no">
      <i class="icon"></i>
    </td>
    
    <td class="no">
      <i class="icon"></i>
    </td>
    
    <td class="yes">
      <i class="icon"></i>
    </td>
  </tr>
</table>

### Show Your Support

If you like the idea of a ubiquitous .NET client application development model, please take the time and let Microsoft know by voting for this idea on UserVoice:

<div class="push-button-container"><div class="push-button">
</div><a class="w-inline-block top-lighting" href="http://visualstudio.uservoice.com/forums/121579-visual-studio/suggestions/10027638-create-a-ubiquitous-net-client-application-develo" target="_blank"><div class="glass-insert" data-ix="blink" style="transition: opacity 500ms ease-in-out; opacity: 0;"></div><img class="push-button-vote-text" src="/images/VoteNow.svg" /></a></div>

 [1]: /2015/10/introduction/#who-are-you-who-is-the-8220we8221
 [2]: /2015/10/ubiquitous-qualities/
 [3]: http://urho3d.github.io/
 [4]: https://powerapps.microsoft.com/en-us/
 [5]: http://www.noesisengine.com/
 [6]: https://github.com/SuperJMN/OmniXAML
 [7]: https://github.com/OmniGUI/OmniGUI
 [8]: http://forums.dotnetfoundation.org/t/wasm-asm-js-plans-projects/1947
 [9]: https://github.com/OmniGUI/OmniGUI/issues/2
 [10]: https://github.com/SteveSanderson/Blazor
 [11]: /2015/10/ubiquitous-qualities/#consistent-user-experience
 [12]: /2015/10/ubiquitous-qualities/#object-serialization-congruence