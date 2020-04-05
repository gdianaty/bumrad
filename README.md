

# [Bumrad for Portal 2](http://bumrad.gmdianaty.com/)
A custom light compiler for Portal 2.

I built this VRAD for internal use on PUNT. The binaires are available to anyone. It is compatible with Hammer. (Note: using this with the Portal 2 Puzzlemaker will achieve no visual effect, because to use the features Bumrad provides you have to pass arguments into the compiler - something that is not possible for Portal 2 Puzzlemaker to my knowledge.)

It includes an Ambient Occlusion baked into the lightmap, allowing for a much more accurate portrayal of the depth of the environment. This technology is transplanted from Counter-Strike: Global Offensive. Such techniques are also used by Desolation, Portal 2: Abyss, Slartibarty's VRAD, Keep Away from Fire's Boreal Alyph and more. It is safe to say that this is the standard.
Just drop `vrad_dll.dll` into the BIN folder of your Portal 2 installation and you're done! Ready to go.

**Download the latest release [here](https://github.com/gdianaty/bumrad/releases).**
**Report your problems [here](https://github.com/gdianaty/bumrad/issues). Not in my DMs. PLEASE.**

## Ambient Occlusion
Provides the illusion of depth in an environment.
- **Pros:**
	- Increases visual fidelity in all environments.
	- Very similar to Screen Space Ambient Occlusion, but with no performance overhead.
- **Cons:**
	- Map compiling now takes roughly twice as long.
	- Can add strange artifacting to your geometry.
	 
Ambient Occlusion is disabled by default, and may be enabled by passing `-bumrad_ao`.

## Softening
Provides a softer lighting look instead of a harsher look.
- **Pros:**
	 - Increases visual fidelity in darker environments such as overgrown Aperture or testing spheres.
 - **Cons:**
	 - Increases compile time by a small amount.
	 - Looks silly on brighter environments, some maps do and don't work with it. I recommend experimenting and **building your map's lighting with this enabled if you plan to use it**.

Light Softening is disabled by default, and may be enabled by passing `-bumrad_soften`.
