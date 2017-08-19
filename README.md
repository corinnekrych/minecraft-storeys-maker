# minecraft-storeys-maker

Minecraft extension to make your own stories in, with and for Minecraft - it's like being a movie director!

_TODO_ **YouTube video here...** <!-- https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet#youtube-videos -->

Licensed under the [GNU Affero General Public License v3.0 (AGPLv3)](LICENSE).  Contributions most welcome.

Please do Star & Watch this GitHub project if you like it!

## Get it

_TODO Download this Mod's JAR file from_ **CI link TBD**

Place it into your [spongepowered.org](https://www.spongepowered.org) Minecraft, e.g. the mods/ directory of a Vanilla server.

## Use it

Write your own .story file, e.g. see [hello.story](narrate/src/main/resources/hello.story).

Run it with `/story <story-name>` (without .story suffix, so e.g. `/story hello`)

## Story syntax

    # Comment
    // also comment

    = Title
    == Subtitle

    /tp 0 0 0

    This is something which will appear on the chat.

    @entityName this is something that the entity will "narrate" (in its name tag, like a speech bubble in a cartoon)
    you can use more than one line; everything until the next paragraph break (double new line) will be part of the narration.
    You do not have to break up the text yourself - it will automatically be "chopped up" appropriately by itself.

    Now this will appear on the chat again (unless there is a '@' character in front again).

You can of course use ANY Minecraft command in any line that starts with the '/' character, not just /tp.

An entity's name must be given to your actors with a naming tag (via an Anvil), as always in normal Minecraft.

You can obviously mix the order and repeat titles, comments, chats, narrations and commands.

## Commands

* `/story <story-name>` plays a story, read from config/storeys/stories/<story-name>.story
* `/narrate <entityName> Text..` makes an entity "narrate" the _Text_

## FAQ

**Seriously, "storeys" (not _"stories"_), are you mental?** Yeah.. just to avoid any possible confusion with Minecraft Story Mode! ;-)
