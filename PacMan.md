# Pac-Man


Startup cruft
  18x14 grid (full-screen top-to-bottom)
  ghost names give clues
  shows the score for eating ghosts
  ...increase incrementally
  shows that eating a pellet makes ghosts edible
  shows value of pellets


Game Start
  music and wait-time that shows High-Score

Game Screen
  Open Maze
    open paths
    walls, blocked paths
  teleport off edge of screen to opposite edge
    only access two locations on sides

Movement
  it goes the direction but it doesn't turn until you tap a direction

Pac-Man
  yellow
  
  eat all four ghosts = extra life
  eat all pellets = new level
  death ~ return to start position, ?bottom-middle below fruit

  animation
    moving & mouth chomps
    stopped ~ mouth stays where it was
    dying
    mouth points in the direction of travel
  sounds
    moving
    eating pellet: large & small
    eating ghost
    dying


Ghost
  timer to release ghosts one at a time
  slightly faster than pac-man
  4 ghosts
    each with personality
      red, Shadow, Blinky ~ aggressive
      pink, Speedy, Pinky ~ indirect to trap player
      cyan, Bashful, Inky ~ 
      orange, Pokey, Clyde ~ seeks player then runs away

  when a large pellet the ghosts become dark-blue & edible
    dark-blue ghost ~ vulnerable to being eaten
    ...can be eaten
    when eaten the game pauses for a bit
    can be turned while in ghost-house

  if the player is too far away they return to their corner and orbit
  after being eaten they return the the center/ghost-house

  animations
    movement
    eyes look in the direction of travel
    edible
      blue
      after a time they flash blue/white indicating almost inedible again
    eyeballs after being eaten
  sounds
    movement

Between Level
  animation

Pac-Man and ghosts speed-up a little bit on each level

Points
  fruit 300
  ghosts 200, 400, 800, 1600
  pellets 10, 50


HUD
  Number of lives remainin at bottom
  Level = number of icons lower-right (?fruit?)
  score ~ top-left
