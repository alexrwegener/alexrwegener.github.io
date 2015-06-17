---
layout: post
title: "Clean Apps with Dagger 2"
modified: 2015-06-17T08:31:55-05:00
categories: blog
excerpt: 
tags: [Android, Presentation]
image:
  feature:
date: 2015-06-17T08:31:55-05:00
share: true
---

{% highlight java %}
public final class IndyGDG {
   private final Devs devs;
   private final Location location;
   private final Speaker speaker;
   public IndyGDG() {
       this.devs = new AndroidEnthusiasts();
       this.location = new DeveloperTown();
       this.speaker = new AlexWegener();
   }
   public void meetup() {
       location.host();
       do {
           speaker.present();
       } while (devs.areEatingPizza());
   }
}
{% endhighlight %}

Last night I presented on creating clean apps with Dagger 2 at the Indianapolis GDG. It was an exhilarating experience as it was my first presentation ever! I was very excited about the turnout (~20 people) but there was also a video recording (coming soon!) for those of you weren't able to make it. Check out the [slides](https://speakerdeck.com/alexrwegener/clean-apps-with-dagger-2) and the sample scope app on [Github](https://github.com/alexrwegener/dagger2-scopes) if you are so inclined.