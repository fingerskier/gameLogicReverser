# Asteroids

starts up on the game screen

Player
  Controls
    left, right, thruster, shoot, hyperspace

  player rotate left and right
  ...and move in the direction they are pointing
  ...once moving they can turn and it preserves momentum

  player goes off one side of the screen they come in the opposite side

  player pushes button and shoots bullets

  after destruction
    player respawns when hitting the button
    player respawns dead-center
    spawn X large asteroids at the edges of the screen
      X ~= level-number

  hyperspace
    hold hyperspace ~ leaves player in limbo
    release hyperspace ~ move player to a random location on screen
    ...danger of moving directly into the path of something

  animations
    turning
    destruction

Sounds
  shooting
  thrusters
  asteroid hits
  UFO hits
  UFO travel
    different sounds ?= different value

Bullets
  only 3 bullets on-screen at a time
  bullets are separate objects
  bullets also teleports off the screen edges
  after hitting something the bullet disappears

Asteroids
  when bullet hit large asteroids those become 2 medium asteroids
  when bullet hit medium asteroids those become 2 small asteroids
  when bullet hit small asteroids those are destroyed
  ...destruction or breaking up has a shrapnel animation

  the smaller the asteroid, the faster it travels

  asteroids do not contact each other

  asteroids also teleports off the screen edges

  animations
    turning
    destruction
    
Teleporting
  when an object goes "off" the edge of the screen it appears on the opposite edge of the screen

UFOs
  shoots at the player
  when shot the UFO blows up
  random spawn, maybe more at higher levels?
  ?don't teleport?
  ?time limit?
  don't turn
  can destroy asteroids and the player
  when a UFO shoots an asteroid there are no points awarded but the asteroid does get destroyed

  animations
    destruction

Level End
  when all asteroids are destroyed, clears to new level (?more asteroids than previous)


HUD
  shows score & lives

Lives
  getting once = player destruction = lose a life

Score
  large = 50
  medium = 50
  small = 100
  UFO = 100
  extra life
    based on points?
      10000, 20000, 40000,

Death Screen
  your score
  your ranking
  enter initials