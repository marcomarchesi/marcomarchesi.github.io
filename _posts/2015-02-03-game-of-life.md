---
layout: post
title: Game of Life
categories: games iOS
date:   2015-02-03 13:51:53
tags: []
published: True

---

It's a long time that I was thinking to create an implementation of the Game of Life. Created in 1970 by John Conway, it's the most popular example of automata.


{% highlight objective-c %}
    // Create audio player for background
    NSString *backgroundMusicPath = [[NSBundle mainBundle] pathForResource:@"gameoflife" ofType:@"caf"];
    NSURL *backgroundMusicURL = [NSURL fileURLWithPath:backgroundMusicPath];
    self.backgroundMusicPlayer = [[AVAudioPlayer alloc] initWithContentsOfURL:backgroundMusicURL error:nil];
    self.backgroundMusicPlayer.delegate = self;
    self.backgroundMusicPlayer.volume = 0.1;
    self.backgroundMusicPlayer.numberOfLoops = -1;  //no loops
    [self.backgroundMusicPlayer play];
{% endhighlight %}