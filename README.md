# Easing functions for Godot (v3.2)

![LOGO](/icon.png)

Bring the powerful easing functions to godot

## Usage

Copy the script in your project resource folder and call them as:

> Easing.[TYPE].[FUNC](t, b, c, d)

inside your code.

example:

    var t = 0
    
    func _process(delta):
        t += delta
        position.x = Easing.Expo.EaseOut(t, 0.0, 100.0, 3.0)

this moves on the x axis an object from position 0.0 to position 100.0 in 3 seconds decreasing the speed exponentially.

#### TYPE available

- `Back`
- `Bounce`
- `Circ`
- `Cubic`
- `Elastic`
- `Expo`
- `Linear`
- `Quad`
- `Quart`
- `Quint`
- `Sine`

#### FUNC available

- `EaseIn`
- `EaseOut`
- `EaseInOut`
- `EaseOutIn`
- `EaseNone` (just for `Linear` type)

(For `Linear` type all FUNC are the same)

## Useful resources

- Prewiev easing functions (https://easings.net/)
- Original Robert Penner's Easing Functions at http://robertpenner.com/easing/
- Original Terms of Use: http://robertpenner.com/easing_terms_of_use.html
