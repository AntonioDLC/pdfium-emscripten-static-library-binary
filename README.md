Credits to https://github.com/bblanchon/pdfium-binaries for figuring out how to perfectly build pdfium for everyone else in the world.
   
What makes this particular binary different than the one automatically built by pdfium-binaries is that it avoids the pthread/atomics/bulk-memory error when linking it against an emscripten project with pthread functionality enabled.
That's it (and also that the debug symbols are already stripped).
