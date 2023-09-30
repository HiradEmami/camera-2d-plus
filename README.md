# Camera2D+
The "Camera2D+" plugin enhances the functionality of the built-in Camera2D node in Godot, providing additional features for game camera management. With Camera2D+, you can easily implement screen shake effects, screen flashes, and cinematic mode transitions in your 2D games. Take control of your in-game camera and create immersive and dynamic gameplay experiences with this versatile and user-friendly plugin.

## Camera2D+ Functionalities
Camera2D+ is an enhanced Camera2D node with additional features to elevate your game or project. This plugin provides the following advanced functionalities:

1. ***Screen Shake***:
    - Camera2D+ can simulate screen shaking effects, adding intensity and realism to your game.
    - You can customize the duration, intensity, and type of shaking.
    - It smoothly returns the camera to its original position after the shake, ensuring a seamless transition.

2. ***Screen Flash***:
    - Create stunning visual effects by flashing the screen with Camera2D+.
    - Customize the flash color, duration, and intensity to suit your game's needs.
    - This feature is useful for emphasizing critical moments or creating dramatic effects in your game.

3. ***Follow Node***:
    - Camera2D+ allows you to follow a specific node, even if it's not a direct child of the camera.
    - Easily track your player character or any other object, keeping it in the center of the view.
    - Achieve dynamic camera movement for a more immersive gaming experience.

4. ***Cinematic Mode***:
    - Simulate the cinematic screen effect with Camera2D+ by adding black bars to the corners of the screen.
    - This feature can give your game or project a cinematic feel, mimicking the widescreen format often seen in movies.
    - Customize the size and position of the black bars to achieve the desired cinematic effect.

These powerful functionalities enhance your camera management capabilities, allowing you to create engaging and visually appealing games and projects. Camera2D+ is a valuable addition to your Godot toolkit, offering flexibility and creative control over your camera scenes.

## Camera2D+ Basic Functions
Camera2D+ provides a set of fundamental functions to help you create immersive visual effects in your game or project. Here are the core functions that allow you to generate the screen flash, screen shake, and cinematic effects:

1. ***flash(color: Color = Color.WHITE, duration: float = 0.5, hold: float = 0.0) -> void***:
    - The `flash` function triggers a screen flash effect with the specified `color`. By default, it uses white.
    - You can customize the `duration` of the flash effect, which determines how long the screen will remain flashed.
    - The `hold` parameter allows you to hold the flash effect for an additional duration before it begins to fade out.
    - This function is useful for highlighting important events or creating visual impact.

2. ***add_shake(strength: float) -> void***:
    - The `add_shake` function adds a shaking effect to the camera with the given strength.
    - You can call this function multiple times to intensify the shaking effect. For example, calling it with values 10 and 5 successively will result in a total shaking effect of 15.
    - Use this function to simulate various degrees of camera tremors.

3. ***set_shake(strength: float) -> void***:
    - The `set_shake` function sets the camera's shaking effect to a specific strength.
    - Calling this function more than once will overwrite the previous strength value. For instance, if you call it with values 10 and 5 successively, the total shaking effect will be 5, as the second call overrides the first.
    - Useful to prevent camera shake stacking.

4. ***set_follow_node(new_node_path: NodePath) -> void***:
    - With the `set_follow_node` function, you can designate a new node for the camera to follow.
    - For this feature to work effectively, ensure that the node to be followed is not a child of the camera, and the camera is not its child either.
    - Provide the node's path rather than the node itself to specify the target.

5. ***toggle_cinematic(horizontal: bool, vertical: bool = false) -> void***:
    - The `toggle_cinematic` function activates or deactivates the cinematic effect along the horizontal and vertical axes.
    - If you set `horizontal` to true, it enables the cinematic effect on the horizontal axis.
    - To enable both horizontal and vertical cinematic effects, set `vertical` to true as well.
    - This function is great for creating cinematic moments in your game, adding a touch of professional cinematography.

These core functions provide you with the building blocks to implement captivating visual effects and camera behavior in your Godot projects using the Camera2D+ plugin. Feel free to experiment and combine these functions to achieve your desired results!
