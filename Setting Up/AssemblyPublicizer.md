# Assembly Publicizer
### What is it and why?
An assembly publicizer transforms a dll, changing all fields / properties / methods into there public equivalent. This is useful for modding, as it can often reliably replace reflection, allowing a modder to easily access normally private methods/variables within the games base source.

### How can we use it?
- Download the Assembly Publiciser from [here](https://github.com/CabbageCrow/AssemblyPublicizer)
- Use the commandline interface (as described in the publiciser's github repo), or drag and drop your dll onto the publiciser exe
- You should see a copy of the dll named 'Assembly-CSharp_publicized.dll'
- You can now add this as a reference to your project solution (replacing your old reference)
- Disable 'Allow unsafe code' in your IDE

### Notes
- This will not always work, by nature of what it is (a dirty hack), but it is incredibly useful 90% of the time, it does not constitute as an excuse to not learn C# reflection, as you will likely need both in conjunction at times.

### Basic Mistakes
- Make sure, if you are dragging and dropping your dll, that you drag and drop the original dll, not a copy, if you try with a copy, you will see that your outputted dll will be 0 bytes in size
- Do not replace your Assembly-CSharp.dll with the publicised dll, simply compile against the publisized version

