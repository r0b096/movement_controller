# Movement Controller for Unity

The `MovementController` script is designed for use in Unity to control the movement of a game character. It uses the Unity `CharacterController` component to allow the character to move based on user input.

## Features

- Smooth and responsive character movement.
- Easily configurable movement speed.
- Input from the arrow keys or "W", "A", "S", and "D" keys for both horizontal and vertical movement.

## Usage

1. Attach the `MovementController` script to your character in Unity by dragging and dropping it onto the GameObject with the character.

2. In the Inspector, you can configure the movement speed by adjusting the `speed` variable.

3. Make sure you have a `CharacterController` component attached to your character GameObject. Assign the `CharacterController` to the `controller` variable in the Inspector.

4. Run your Unity game. The character will move in response to the arrow keys or "W", "A", "S", and "D" keys.

## Script Explanation

- The `Update` method constantly checks for user input to move the character.
- It reads the horizontal and vertical input axes using `Input.GetAxisRaw()`.
- It creates a `Vector3` to represent the movement direction by setting the `x` and `z` components based on the input.
- If the magnitude of the `direction` vector is greater than or equal to 0.1 (meaning there's significant input), it moves the character using the `CharacterController.Move` method.

## Contributing

Contributions are welcome! If you'd like to contribute to this project, please follow these guidelines:

1. Fork the repository.
2. Create a new branch: `git checkout -b feature/your-feature-name`.
3. Make your changes and commit them: `git commit -m 'Add some feature'`.
4. Push to the branch: `git push origin feature/your-feature-name`.
5. Open a pull request to the `main` branch of this repository.
