Story Wall
==========

`storywall` is like markdown but for tracking stories in plain text. It's a simple DSL for capturing an easy to edit and highly version controllable story wall.

Think of it a being like Pivotal Tracker or Mingle, but in plain text. Put it in your version control of choice and keep it versioned right alongside your project.

A `storywall` is just a text file that looks like this:

    # storywall example
    #
    # <Column name>:
    #   <Title> [<owner initials>/<initiator initials>] (<tag>:<value>, ...) <Description>
    
    In Progress:
      * User uploads image [ZY/AB] (type:story) Maximum of 3Mb jpg or png's, 2 images allowed
    
    Backlog:
      * User can add image as avatar [ZY/AB] (type:story)
      * Images must not be smaller than 100x100 [ZY/AB] (type:bug)
    
    Next Release:
      * User can upload more than 2 images [AB/ZY] (type:story)
    
    Done:
      * User can login using OAuth [AB/ZY] (type:story)
      * User can add a profile [AB/ZY] (type:story)
      