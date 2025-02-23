---
title: "Reliability: Finding Your Marathon Pace"
layout: post
date: 2025-02-23 22:48
image: /assets/images/slo_availability_table.png
headerImage: false
tag:
- reliability
- service level objectives
category: blog
author: bayneri
description: Can a runner sustain a 10-second-per-100-meter pace for an entire marathon? What if our systems had to do the same? How does this relate to achieving perfection in reliability?
---

The 10-second barrier—completing a 100-meter sprint in under ten seconds—once stood as the ultimate test of human speed, a physical and mental milestone reserved for elite sprinters. But its significance has faded since the late 1990s as more athletes have crossed the finish line in less than ten seconds. To date, 199 sprinters have officially broken this barrier. It’s impressive, but no longer impossible.

Now, consider a marathon: 42,195 meters long endurance test. Could a human sustain that 10-second-per-100-meter pace across such a distance? Simple math suggests a marathon at this speed would take just 1 hour, 10 minutes, and 19.5 seconds—an average of 10 meters per second, or 36 kilometers per hour, for over an hour. In reality, this is far beyond human limits. The men’s marathon world record, set by Kenyan runner Kelvin Kiptum at the 2023 Chicago Marathon, is 2 hours, 0 minutes, and 35 seconds. That’s an average of 5.86 meters per second (21.1 kilometers per hour), or roughly 17 seconds per 100 meters. Even the best of the best can’t sprint a marathon.

So why are we talking about running? Because the contrast between a sprint and a marathon mirrors a critical lesson in system reliability and Service Level Objectives (SLOs). Short bursts of excellence are one thing; sustained performance is another—and SLOs demand we think beyond the finish line of a single race.

## Sprinting vs. Marathon in SLOs
Think of your system as a runner. Nailing a traffic spike with zero downtime is like a sprinter crushing a 100-meter dash—a flashy, short-term win. But true reliability isn’t about one-off heroics; it’s about consistency over weeks, months, or years—the marathon equivalent. Setting an SLO like 100% uptime might sound noble, but it’s like asking a runner to sprint a marathon: it’s unsustainable and risks burning out both your system and your team.
Take an e-commerce platform during Black Friday as an example. A team might aim for 100% uptime for those 24 hours—full speed, like a sprinter pushing for a sub-10-second dash. They add servers, stay up all night, and maybe they win. But extend that expectation across an entire year, and the cracks show: hardware fails, updates glitch, and teams exhaust their reserves. The sprint works for a day; the marathon needs a different strategy.

## Setting Realistic SLOs
Smart SLOs take the long view. Instead of chasing perfection, aim for a target that’s ambitious yet sustainable. A 99.9% uptime goal, for instance, leaves room for minor hiccups—think of them as water breaks in a marathon. Your team doesn’t collapse, and you still have energy to try new ideas. It’s about finding a pace you can maintain, not a speed that leaves you gasping.

Think of Netflix, the streaming giant. An SLO of 99.99% availability for video playback might seem ideal. After all, users expect seamless binge-watching. But that translates to just 4 minutes and 23 seconds of downtime per month. Push it to 100%, and you’re demanding zero outages, which could mean delaying new features (like a shiny recommendation algorithm) to avoid any risk. Instead, Netflix might settle for 99.9%. A mere 43 minutes of wiggle room per month, allowing brief buffering hiccups while still delivering a great experience. The key is aligning the SLO with user tolerance and business goals, not an arbitrary perfect score.

Or take a healthcare app tracking patient vitals. Here, reliability is life-critical. 99.9% might not cut it if it means 8 hours of downtime a year. A 99.99% SLO (less than an hour offline) could be the minimum, balanced against the cost of redundant systems and the reality of occasional maintenance. It’s a faster marathon pace, but still humanly achievable with the right preparation.

![SLO Availability Table](/assets/images/slo_availability_table.png)
<figcaption class="caption">source: https://sre.google/sre-book/availability-table/</figcaption>

## Balancing Performance and Reliability
Marathon runners know the trade-off between speed and endurance. Push too hard, and you crash; waste time for too long, and you miss the mark. Systems face a similar balancing act. Over-optimizing for peak performance can make them fragile, while obsessing over stability might slow progress to a crawl. The sweet spot is a pace that delivers solid performance and keeps the system resilient over time.

Let’s take Uber as an example. During a New Year’s Eve surge, it might hit 99.95% request success for a few hours—drivers are matched lightning-fast, like a sprinter’s burst. But if that SLO were applied year-round, every edge case (GPS glitches, driver shortages) could tip it over. A smarter long-term SLO might be 99.8%, accepting 17 hours of minor hiccups annually—say, a few unmatched rides during rush hour—while keeping the system flexible enough to roll out new features like carpooling. Over-focus on that peak sprint, and you might skip resilience upgrades; over-focus on stability, and riders wait too long. The right pace keeps both wheels turning.

## Conclusion: Run the Right Race
When crafting SLOs, don’t train for a 100-meter dash. Prepare for a marathon. Build systems and set targets that prioritize steady, long-term reliability over fleeting perfection. Whether it’s an e-commerce site weathering holiday spikes, a streaming platform keeping viewers hooked, a healthcare app saving lives, or a ride-sharing service moving millions, the principle holds: match your pace to the distance. That’s how you drive growth, avoid burnout, and win the race that matters.
