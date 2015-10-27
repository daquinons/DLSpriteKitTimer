# DLSpriteKitTimer
Simple Timer for SpriteKit Games written in Swift.

This timer is used in [Elem](http://www.elem.rocks).

## Overview
DLSpriteKitTimer is a subclass of SKLabelNode, so it's ready to be added to any GameScene as a subchild.

It has two modes, being selected in the initializer with the parameter decreasing: Bool
* Decreasing time
* Increasing time

It also allows to set a function executed every second, passing an optional closure to the parameter withActionPersecond: (() -> ())? in the initializer.

It requires a function that is executed at the end of the timer. The parameter is called withFiringAction: () -> () in the initializer.

## API

func start()

func pause()

func stop()

func reset()
