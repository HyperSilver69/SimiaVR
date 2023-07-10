# Normcore

## What you should know
By far the simplest to set up. Hardly takes 20 minutes. However, here is a list of pros and cons to using Normcore.

Pros of using Normcore for VR Multiplayer:

    Accessibility: Normcore offers a more inclusive and accessible experience for VR multiplayer, as it eliminates the need for expensive and specialized VR equipment. Players can join the game using their smartphones or basic devices, making it easier for a larger audience to participate.

    Cost-effective: Since Normcore doesn't require high-end VR equipment, it significantly reduces the cost barrier for players. This can attract a wider range of participants, making the game more financially accessible and potentially increasing the player base.

    Lower system requirements: Normcore's simplified graphics and processing requirements make it compatible with a wider range of devices. Players with lower-end devices can still enjoy the multiplayer experience without needing to upgrade their hardware.

    Social integration: Normcore's accessibility extends to social integration as well. By removing the need for specialized VR equipment, players can easily connect and interact with friends, family, and a broader gaming community, fostering a more social experience.

    Cross-platform compatibility: Normcore's device-agnostic approach allows for cross-platform compatibility. Players using different devices and operating systems can join the same multiplayer game, increasing the potential for diverse and larger player communities.

Cons of using Normcore for VR Multiplayer:

    Reduced immersive experience: Normcore's simplified graphics and lower system requirements mean that the visual and immersive experience might not be on par with high-end VR games. Players might miss out on the level of realism and immersion that VR equipment provides.

    Limited interactions: Normcore's reliance on basic devices like smartphones can limit the range of interactions available in the game. Players might have fewer options for complex movements, gestures, or actions that are possible with specialized VR equipment.

    Performance limitations: Normcore's focus on compatibility across various devices can result in performance limitations. Higher-end devices might not be able to fully utilize their capabilities, while lower-end devices might struggle to deliver a smooth gameplay experience, impacting overall performance.

    Reduced gameplay depth: The simplified nature of Normcore might lead to a reduction in gameplay depth and complexity compared to traditional VR multiplayer games. Players might miss out on intricate mechanics, detailed environments, and advanced features that are only possible with dedicated VR equipment.

    Hardware limitations: While Normcore allows for broader accessibility, it still relies on the capabilities of the player's device. Older or underpowered devices might not be able to run the game smoothly or at all, limiting participation for some potential players.



If you read through those and decided that you want to use Normcore, then you're in the right spot!

Unlike Photon and Mirror, Simia has it's own package for Normcore, making it very simple to set up.

## Setting up Normcore

1. Download the latest Normcore package for Simia [here]()
2. go to [Normcore.io](https://normcore.io/) and create an account.
3. When prompted with four options, select "Create an application", you may name this Application whatever you want. (NOTE TO SELF, INCLUDE THE NORMAL FOLDER IN THE PACKAGE)
4. Copy the ID, then go back into unity.
5. In unity, import the Normcore package (Don't know how? Go back to the [setup](https://github.com/HyperSilver69/SimiaVR/blob/main/Setup.md) page.
6. Go to `Assets -> Normal -> Examples -> VR Player` then drag the `Realtime + VR Player` file into the Player rig, this depends based on which locomotion style you picked.
   - Gorilla tag Locomotion: Drag the file into the `Player` GameObject in your scene.
   - Physics/Capuchin Locomotion: Open the `PhysicsPlayer` GameObject by pressing the arrow next to it, then drag the file into the `Player Rig` Child GameObject.
  Select the GameObject that you just added, and paste the App Key you copied into the `App Key` field in the inspector.
7. Select the `Resources` folder under the `VR Player` folder and open the Prefab called `VR Player`. Here you can change the way the Player looks. Further down in this Setup guide, it will also be where you can apply some of the tutorials!
8. Go back out of the `VR Player` Prefab by pressing the arrow in the top left. Open the same GameObject where you pasted the App Key, and open the `Local Player` dropdown. If the `Local Avatar Prefab` says **none**, then drag the VR Player Prefab into there, otherwise ignore this step.
9. For the Root, depending on your Locomotion style, this is either going to be:
  - Gorilla Tag Locomotion: "GorillaPlayer", this is under the `Player` GameObject.
  - Physics/Capuchin Locomotion: "Camera Offset", this is under the `Player Rig` Gameobject.
10. The `Head` should be the Main Camera, which should be the first thing you see if you press the arrow next to the GameObject which you made the root.
11. The `Left hand` and `Right hand` should be the `LeftHand Controller` and `RightHand Controller` respectively. These are in the same place as the Main Camera.


That's it! You're done setting up Normcore. If you have any issues, please ask in the `Normcore` channel on the [discord](https://discord.gg/ME7UY9vYQD).

## Resources

Here are a few helpful resources when continuing on with Normcore!
[3D player Model for Normcore](https://www.youtube.com/watch?v=tAN6VYmRAE8&t=236s)
[Cosmetics for Normcore](https://www.youtube.com/watch?v=eE_fSh2u4JI)
[Day night cycle](https://www.youtube.com/watch?v=Dk9oDHYvyWk)


