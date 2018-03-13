DependencyAnalyser

Features:
- Language agnostic
- Generate Graph visualization (graphviz dot)
- Check dependencies


Dependencies Definition
---------------------------------------------------



Examples
---------------------------------------------------

Java classes

ClassA:
  classname: mypackage1.ClassA

mypackage1.ClassB:
  classname: mypackage1.ClassB

mypackage2.ClassB:
  classname: mypackage2.ClassB

ClassC:
  classname: mypackage1.ClassC

mypackage1:
  labels: [package]

mypackage2:
  labels: [package]

ClassA -> mypackage1.ClassB
mypackage2.ClassB -> ClassC



mypackage1.* in lib





Haskell Modules
Main (App1.js):
  module: Main
  filename: App1.hs

Main (App2.js):
  module: Main
  filename: App2.hs

MyPkg.MyMod:
  module: MyPkg.MyMod
  filename: MyPkg/MyMod.hs

Lib.Mod1:
  module: Lib.Mod1


Main (App1.hs) -> MyPkg.MyMod
Main (App2.hs) -> MyPkg.MyMod
Mypkg.MyMod -> Lib.Mod1






