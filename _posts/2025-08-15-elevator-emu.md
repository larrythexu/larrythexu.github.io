---
title: "Spring Elevator Emulator :elevator:"
layout: post
date: 2025-08-15
headerImage: false
projects: true
hidden: false
description: "An elevator emulator built in Spring"
category: project
author: Lawrence Xu
externalLink: false
---

Tools and Skills:
 - Java
 - Spring Boot
 - REST API
 - WebSockets

 [Github Link](https://github.com/larrythexu/SpringElevator)

 ---

Whenever I've waited a second too long for an elevator, I always found myself wondering how the software worked. What better way to explore than to try and emulate it myself. It is currently still IN THE WORKS.

I opted to use Spring Boot because of my experience with it, how much already is set up when creating the project, and the swappable beans - in case I wanted to change the selection algorithm for my elevators.

As of right now, the elevator logic and API is implemented. Users can request floors to a floor manager, which then picks an elevator. The elevators registered in the system will move floor-by-floor, dropping off on any of their target destinations. I even took the time to write a bunch of unit tests. 

I did have to explore websockets, which is something I've never worked with. I obviously didn't want to continually send requests for elevator states if I wanted a front-end to keep track of the elevators. I actually wasn't aware of how else it was done, so this was enlightening to learn.

I plan to add more algorithms to see more of a selection variety. There also needs to be a front-end... *gulp*

The Elevator Manager Controller:
{% highlight java %}
@RestController
@AllArgsConstructor
public class ElevatorManagerController {

  private final ElevatorManager elevatorManager;

  @GetMapping("/elevators/{id}")
  public Elevator getElevator(@PathVariable("id") int id) {
    return elevatorManager.getElevator(id);
  }

  @GetMapping("/elevators")
  public List<Elevator> getElevators() {
    return elevatorManager.getAllElevators();
  }
  /** more stuff below **/
}
{% endhighlight %}

