# CrystalMpq is a MPQ reading library written in C#. #
The source code is released under the [Ms-RL](http://www.microsoft.com/opensource/licenses.mspx#Ms-RL) licence.

_If you're not a developper you'll probably be interrested in [CrystalMpq Explorer](CrystalMpqExplorer.md) which lets you access to the files in mpq archives or in a whole WoW installation, or in WoWMapExplorer which lets you browse the 2D maps usually shown in-game._


This project consists of the library and tools written around it:

  * **CrystalMpq** is the core library. This is definitely the one you need if you want to read data from MPQ. Data is accessed using standard .NET streams, meaning the library should be useable with all CLS compliant languages. (Partial support for MPQ up to version 4, patch archives **are** supported)
  * **CrystalMpq.Utility** is a library with extensions allowing for Mpq file systems, and support for WoW installation detection. (Support for WoW 4.0+)
  * **CrystalMpq.Utility.Windows.Forms** is a library extending the previous one (separated from it in order to allow UI toolkit independence), managing an user interface for language pack selection. (WoW file system only)
  * **CrystalMpq.DataFormats** is a library giving support for some WoW file formats. Currently supported are DBC, BLP1 (War III) and BLP2 (WoW).
  * **CrystalMpq.WoWDatabases** is the most recent library, containing only definitions for some specific DBC files, as well as some spell information found here and there. (Aura names, Effect names)
  * **CrystalMpqExplorer** is an extensible Windows Forms interface that will let you explore MPQ files.
  * **WoWMapExplorer** will let you view WoW's world map in an Windows Forms user interface, streaming the map data directly from the wow installation.
  * **DbcViewer** is a standalone DBC reader provided for viewing DBC files outside of the MPQ explorer UI.
  * **WoWSpellViewer** is a test project for viewing Spell Data contained in MPQ files. It is not likely to work for now, as the database format has to be kept in sync with WoW quite frequently. (_As of now, it will just not work at all, since the spell database ahs been split up in many smaller ones._)


I started this project around 2005, and upgraded it regularly until I got something working decently. There, from refactoring to refactoring, and by adding features bit by bit, I finally got something quite pleasant for my own use.
I never released the source code before 2011, but it has now been done.
I am still upgrading the project from time to time, so you can expect progressive upgrades as long as I'm not dead…

If you like this project, please spread the word !

Thanks