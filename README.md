
# [Bumrad for Portal 2](http://bumrad.gmdianaty.com/)
A custom light compiler for Portal 2.

I love to see things created using the Source Engine. Because the developers of the engine abandoned it long ago, I only get to see amazing things created by the community. A personal commitment of mine is to help the community create amazing things. Portal 2 is often under-loved and under-appreciated by us Source Engine licensees. I like to try and help when I can.

I built this VRAD for PUNT internal use. However, I believe it's only right for the whole community to benefit from this creation. It is compatible with the Puzzlemaker, and Hammer Level Editor. You don't need to credit me. Just make something amazing **in the name of science**.

It includes an Ambient Occlusion baked into the lightmap, allowing for a much more accurate portrayal of the depth of the environment. This technology is transplanted from Counter-Strike: Global Offensive. Such techniques are also used by Desolation, Portal 2: Abyss, Slartibarty's VRAD, Keep Away from Fire's Boreal Alyph and more.
Just drop `vrad_dll.dll` into the BIN folder of your Portal 2 installation and you're done! Ready to go.

**Download the latest release [here](https://github.com/gdianaty/grahams-compiler-tools/releases).**
**Report your problems [here](https://github.com/gdianaty/grahams-compiler-tools/issues). Not in my DMs. PLEASE.**

## Ambient Occlusion
Provides the illusion of depth in an environment.
- **Pros:**
	 - Increases visual fidelity in all environments.
	 - Very similar to Screen Space Ambient Occlusion, but with no performance overhead.

AO is enabled by default, you may disable it with `-no_AO`.

## Softening
Provides a softer lighting look instead of a harsher look.
- **Pros:**
	 - Increases visual fidelity in darker environments such as overgrown Aperture or testing spheres.
 - **Cons:**
	 - Increases compile time by a small amount.
	 - Looks silly on brighter environments, some maps do and don't work with it. I recommend experimenting.

Softening is disabled by default, you may enable it with `-soften`.
