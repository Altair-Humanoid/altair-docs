= Ubuntu install of ROS Noetic =

[[http://build.ros.org|The ROS build farm]] builds Debian packages for several Ubuntu platforms, listed below. These packages are ready to use so you [[noetic/Installation/Source|don't have to build from source]]. You can check the status of individual packages [[http://repositories.ros.org/status_page/ros_noetic_default.html|here]].


{{{#!wiki solid/blue
Note that there are also packages available from Ubuntu upstream. Please see [[UpstreamPackages]] to understand the difference.
}}}

<<Include(SupportBuildfarm)>>

<<TOC(3)>>


== Installation ==

<<Include(Installation/Ubuntu/Sources)>>


=== Installation ===

<<Include(noetic/Installation/DebianMetapackages)>>

<<Include(noetic/Installation/DebEnvironment)>>

=== Dependencies for building packages ===
Up to now you have installed what you need to run the core ROS packages. To create and manage your own ROS workspaces, there are various tools and requirements that are distributed separately. For example, [[rosinstall]] is a frequently used command-line tool that enables you to easily download many source trees for ROS packages with one command.

To install this tool and other dependencies for building ROS packages, run:

{{{
sudo apt install python3-rosdep python3-rosinstall python3-rosinstall-generator python3-wstool build-essential
}}}


==== Initialize rosdep ====

Before you can use many ROS tools, you will need to initialize `rosdep`. `rosdep` enables you to easily install system dependencies for source you want to compile and is required to run some core components in ROS. If you have not yet installed `rosdep`, do so as follows.

{{{
sudo apt install python3-rosdep
}}}

With the following, you can initialize `rosdep`.

{{{
sudo rosdep init
rosdep update
}}}

<<Include(noetic/Installation/PostInstall)>>

== ROS One-line Installation ==
Check out [[http://wiki.ros.org/ROS/Installation/TwoLineInstall/|this tutorial]] to install ROS Noetic using a single command.