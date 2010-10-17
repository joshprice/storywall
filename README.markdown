Story Wall
==========

`storywall` is like markdown but for tracking stories in plain text. It's a simple DSL for capturing an easy to edit and highly version controllable story wall.

Think of it a being like [Pivotal Tracker](http://www.pivotaltracker.com/) or [Mingle](http://www.thoughtworks-studios.com/mingle-agile-project-management), but in plain text. Put it in your version control of choice and keep it versioned right alongside your project.

A `storywall` is just a text file that looks like this:

    # storywall example
    #
    # <Column name>:
    #   <Title> [<owner initials>/<initiator initials>] (<tag>:<value>, ...) <Description>
    
    In Progress:
      * User uploads image [ZY/AB] (type:story) Maximum of 3Mb jpg or png's, 2 images allowed
      * Install imagemagick on server [AB/AB] (type:chore) Don't forget to document all steps
    
    Backlog:
      * User can add image as avatar [ZY/AB] (type:story)
      * Images must not be smaller than 100x100 [ZY/AB] (type:bug)
    
    Next Release:
      * User can upload more than 2 images [AB/ZY] (type:story)
    
    Done:
      * User can login using OAuth [AB/ZY] (type:story)
      * User can add a profile [AB/ZY] (type:story)
      

Why would I use storywall over a more fancy tool?
-------------------------------------------------

* You like simple tools
* The format can be as simple or as complex as you like
* Your data is in a format that anybody can understand
* You can edit your storywall with whatever tool you like to edit text with
* In other words you don't need to learn another tool
* Your storywall is versioned and distributed right alongside your code so you know your history is always there when you need it
* Text is regular and parsable, like a text-based API
* You can extend the format if it doesn't have the feature you want

How do I get started?
---------------------

`storywall` is currently just a spec, but you can use it right now!

Just create a file called `project.storywall` in your project directory. Use the file format above and make sure it's version controlled.

To move a task between states, simply move the line.

When you're done editing, commit and push the result so the rest of your team can see the progress.

If you get a merge conflict just resolve as you normally would. You might want to check with your team member to make sure no data was lost in the merge.


What's next?
------------

I'm planning to build some basic tools around this in order to produce burn-up/down charts collect some other statistics from your project storywall.

At this stage it'll likely be a rubygem with some scripts which allow you to visualise, import and export your storywall data.

Currently I'm soliciting feedback. So if you like the spec or have any comments, ideas or questions, please let me know!

