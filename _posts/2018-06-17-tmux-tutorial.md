---
layout: post
title: "Tmux Guide"
description: "Description of tmux with necessary commands"
date: 2016-08-15
tags: programming command_line
---

For the last three years, I prefer to work with command line. I do not know why, but I love to write all installation commands there, make commits and push to repositories in a terminal. Also, I tried to learn Vim with its commands but it was not effective for me because I tried to use it as my default editor in daily tasks. Due to unknowing this stuff, it was very bad.

And now I want to go deeper and I will start with **tmux** - `terminal multiplexer`. It allows you to create as many terminal windows as you want in one window and split-views (in tmux terminology it called 'panes'). 

# Getting started

## Installation

#### Ubuntu and derivatives
```shell
sudo apt-get install tmux
```
#### Mac
```shell
brew install tmux
```

## Starting first session
Type the following in your terminal window:
```shell
tmux
```
<p align="center">
  <img src="https://github.com/kgusman/kgusman.github.io/blob/master/assets/tmux/tmuxFirstSession.png?raw=true">
</p>

## Panes commands

<table style="width:100%">
  <tr>
    <th>Command</th>
    <th>Shortcut</th>
  </tr>
  <tr>
    <td>Split vertically</td>
    <td>Ctrl-b %</td>
  </tr>
  <tr>
    <td>Split horizontally</td>
    <td>Ctrl-b "</td>
  </tr>
  <tr>
    <td>Navigating panes</td>
    <td>Ctrl-b < arrow key ></td>
  </tr>
  <tr>
    <td>Close pane</td>
    <td>Ctrl-d</td>
  </tr>
</table>
<p align="center">
  <img src="https://github.com/kgusman/kgusman.github.io/blob/master/assets/tmux/tmuxFirstPane.png?raw=true">
</p>
<p align="center">
  <img src="https://github.com/kgusman/kgusman.github.io/blob/master/assets/tmux/tmuxSecondPane.png?raw=true">
</p>

## Windows

<table style="width:100%">
  <tr>
    <th>Command</th>
    <th>Shortcut</th>
  </tr>
  <tr>
    <td>Create new tmux window</td>
    <td>Ctrl-b c</td>
  </tr>
  <tr>
    <td>Switch to `previous` window</td>
    <td>Ctrl-b p</td>
  </tr>
  <tr>
    <td>Switch to `next` window</td>
    <td>Ctrl-b n</td>
  </tr>
  <tr>
    <td>Switch to window by number</td>
    <td>Ctrl-b < number ></td>
  </tr>
  <tr>
    <td>Detach current session (window)</td>
    <td>Ctrl-b d</td>
  </tr>
</table>

## Session handling
Detaching does not close your window completely. If you did that by mistake you can enter
```shell
tmux ls
```
to see all your detached windows and restore the necessary window by typing:
```shell
tmux attach -t <window number from the list>
```