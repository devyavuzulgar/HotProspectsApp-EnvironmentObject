# HotProspectsApp-EnvironmentObject

In this tutorial by Paul Hudson, I learned how to use @EnvironmentObject in SwiftUI.

@EnvironmentObject - Note: Imagine we had multiple views in an app, all lined up in a chain: view A shows view B, view B shows view C, C shows D, and D shows E. View A and E both want to access the same object, but to get from A to E you need to go through B, C, and D, and they don't care about that object. If we were using @ObservedObject we'd need to pass our object from each view to the next until it finally reached view E where it could be used, which is annoying because B, C, and D don't care about it. With @EnvironmentObject view A can put the object into the environment, view E can read the object out from the environment, and views B, C, and D don't have to know anything happened – it's much nicer.
