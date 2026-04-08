
- [x] #YOUTUBE
- [ ] NEXT
- [ ] PLAYLIST :tada:





Line breaks
If you're writing in issues, pull requests, or discussions in a repository, GitHub will render a line break automatically:

This example
Will span two lines
However, if you are writing in an .md file, the example above would render on one line without a line break. To create a line break in an .md file, you will need to include one of the following:

Include two spaces at the end of the first line.

This example  
Will span two lines
Include a backslash at the end of the first line.

This example\
Will span two lines
Include an HTML single line break tag at the end of the first line.

This example<br/>
Will span two lines
If you leave a blank line between two lines, both .md files and Markdown in issues, pull requests, and discussions will render the two lines separated by the blank line:

This example

Will have a blank line separating both lines
Images
You can display an image by adding ! and wrapping the alt text in [ ]. Alt text is a short text equivalent of the information in the image. Then, wrap the link for the image in parentheses ().

![Screenshot of a comment on a GitHub issue showing an image, added in the Markdown, of an Octocat smiling and raising a tentacle.](https://myoctocat.com/assets/images/base-octocat.svg)

Screenshot of a comment on a GitHub issue showing an image, added in the Markdown, of an Octocat smiling and raising a tentacle.

GitHub supports embedding images into your issues, pull requests, discussions, comments and .md files. You can display an image from your repository, add a link to an online image, or upload an image. For more information, see Uploading assets.

Note

When you want to display an image that is in your repository, use relative links instead of absolute links.

Here are some examples for using relative links to display an image.

Context	Relative Link
In a .md file on the same branch	/assets/images/electrocat.png
In a .md file on another branch	/../main/assets/images/electrocat.png
In issues, pull requests and comments of the repository	../blob/main/assets/images/electrocat.png?raw=true
In a .md file in another repository	/../../../../github/docs/blob/main/assets/images/electrocat.png
In issues, pull requests and comments of another repository	../../../github/docs/blob/main/assets/images/electrocat.png?raw=true
Note

The last two relative links in the table above will work for images in a private repository only if the viewer has at least read access to the private repository that contains these images.

For more information, see Relative Links.

The Picture element
The <picture> HTML element is supported.

Lists
You can make an unordered list by preceding one or more lines of text with -, *, or +.

- George Washington
* John Adams
+ Thomas Jefferson
Screenshot of rendered GitHub Markdown showing a bulleted list of the names of the first three American presidents.

To order your list, precede each line with a number.

1. James Madison
2. James Monroe
3. John Quincy Adams
Screenshot of rendered GitHub Markdown showing a numbered list of the names of the fourth, fifth, and sixth American presidents.

Nested Lists
You can create a nested list by indenting one or more list items below another item.

To create a nested list using the web editor on GitHub or a text editor that uses a monospaced font, like Visual Studio Code, you can align your list visually. Type space characters in front of your nested list item until the list marker character (- or *) lies directly below the first character of the text in the item above it.

1. First list item
   - First nested list item
     - Second nested list item
Note

In the web-based editor, you can indent or dedent one or more lines of text by first highlighting the desired lines and then using Tab or Shift+Tab respectively.

Screenshot of Markdown in Visual Studio Code showing indentation of nested numbered lines and bullets.

Screenshot of rendered GitHub Markdown showing a numbered item followed by nested bullets at two different levels of nesting.

To create a nested list in the comment editor on GitHub, which doesn't use a monospaced font, you can look at the list item immediately above the nested list and count the number of characters that appear before the content of the item. Then type that number of space characters in front of the nested list item.

In this example, you could add a nested list item under the list item 100. First list item by indenting the nested list item a minimum of five spaces, since there are five characters (100. ) before First list item.

100. First list item
     - First nested list item
Screenshot of rendered GitHub Markdown showing a numbered item prefaced by the number 100 followed by a bulleted item nested one level.

You can create multiple levels of nested lists using the same method. For example, because the first nested list item has seven characters (␣␣␣␣␣-␣) before the nested list content First nested list item, you would need to indent the second nested list item by at least two more characters (nine spaces minimum).

100. First list item
     - First nested list item
       - Second nested list item
Screenshot of rendered GitHub Markdown showing a numbered item prefaced by the number 100 followed by bullets at two different levels of nesting.

For more examples, see the GitHub Flavored Markdown Spec.

Task lists
To create a task list, preface list items with a hyphen and space followed by [ ]. To mark a task as complete, use [x].

- [x] #739
- [ ] https://github.com/octo-org/octo-repo/issues/740
- [ ] Add delight to the experience when all tasks are complete :tada:
Screenshot showing the rendered version of the markdown. The references to issues are rendered as issue titles.

If a task list item description begins with a parenthesis, you'll need to escape it with \:

- [ ] \(Optional) Open a followup issue

For more information, see About tasklists.

Mentioning people and teams
You can mention a person or team on GitHub by typing @ plus their username or team name. This will trigger a notification and bring their attention to the conversation. People will also receive a notification if you edit a comment to mention their username or team name. For more information about notifications, see About notifications.

Note

A person will only be notified about a mention if the person has read access to the repository and, if the repository is owned by an organization, the person is a member of the organization.

@github/support What do you think about these updates?

Screenshot of rendered GitHub Markdown showing how the team mention "@github/support" renders as bold, clickable text.

When you mention a parent team, members of its child teams also receive notifications, simplifying communication with multiple groups of people. For more information, see About organization teams.

Typing an @ symbol will bring up a list of people or teams on a project. The list filters as you type, so once you find the name of the person or team you are looking for, you can use the arrow keys to select it and press either tab or enter to complete the name. For teams, enter the @organization/team-name and all members of that team will get subscribed to the conversation.

The autocomplete results are restricted to repository collaborators and any other participants on the thread.

Referencing issues and pull requests
You can bring up a list of suggested issues and pull requests within the repository by typing #. Type the issue or pull request number or title to filter the list, and then press either tab or enter to complete the highlighted result.

For more information, see Autolinked references and URLs.

Referencing external resources
If custom autolink references are configured for a repository, then references to external resources, like a JIRA issue or Zendesk ticket, convert into shortened links. To know which autolinks are available in your repository, contact someone with admin permissions to the repository. For more information, see Configuring autolinks to reference external resources.

Uploading assets
You can upload assets like images by dragging and dropping, selecting from a file browser, or pasting. You can upload assets to issues, pull requests, comments, and .md files in your repository.

Using emojis
You can add emoji to your writing by typing :EMOJICODE:, a colon followed by the name of the emoji.

@octocat :+1: This PR looks great - it's ready to merge! :shipit:

Screenshot of rendered GitHub Markdown showing how emoji codes for +1 and shipit render visually as emoji.

Typing : will bring up a list of suggested emoji. The list will filter as you type, so once you find the emoji you're looking for, press Tab or Enter to complete the highlighted result.

For a full list of available emoji and codes, see the Emoji-Cheat-Sheet.

Paragraphs
You can create a new paragraph by leaving a blank line between lines of text.

Footnotes
You can add footnotes to your content by using this bracket syntax:

# # hello

import { WebSocketServer } from "ws";

const wss = new WebSocketServer({ port: 3002 });

client.on("update", (update) => {
  wss.clients.forEach(ws => {
    ws.send(JSON.stringify(update));
  });
});
https://github.com/YOUTUBEGITS/Aicrafts

PART1 

https://github.com/MINTMETOKEN/WWW.MINTME.COM

# drop-list

https://github.com/YOUTUBEGITS/emoji-cheat-sheet

# emoji-cheat-sheet

[![Up to Date]([Video.Guru_20260103_120300824.mp4](https://github.com/user-attachments/assets/528d88af-5631-4aca-9d36-e4a90ba075ea))]([https://youtube.com/playlist?list=PL9gYSL74h0Ig8kz1x5WPzgJ6L-VIlKEb7&si=Ay6yarSWW2rupp6Y](https://github.com/user-attachments/assets/528d88af-5631-4aca-9d36-e4a90ba075ea))

This cheat sheet is automatically generated from [GitHub Emoji API](https://api.github.com/emojis) and [Unicode Full Emoji List](https://unicode.org/emoji/charts/full-emoji-list.html).
<img width="4096" height="2304" alt="Image" src="https://github.com/user-attachments/assets/528d88af-5631-4aca-9d36-e4a90ba075ea" />
## Table of Contents

- [Smileys & Emotion](#s1mileys--emotion)
- [People & Body](#people--body)
- [Animals & Nature](#animals--nature)
- [Food & Drink](#food--drink)
- [Travel & Places](#travel--places)
- [Activities](#activities)
- [Objects](#objects)
- [Symbols](#symbols)
- [Flags](#flags)
- [GitHub Custom Emoji](#github-custom-emoji)

### Smileys & Emotion

- [Face Smiling](#face-smiling)
- [Face Affection](#face-affection)
- [Face Tongue](#face-tongue)
- [Face Hand](#face-hand)
- [Face Neutral Skeptical](#face-neutral-skeptical)
- [Face Sleepy](#face-sleepy)
- [Face Unwell](#face-unwell)
- [Face Hat](#face-hat)
- [Face Glasses](#face-glasses)
- [Face Concerned](#face-concerned)
- [Face Negative](#face-negative)
- [Face Costume](#face-costume)
- [Cat Face](#cat-face)
- [Monkey Face](#monkey-face)
- [Heart](#heart)
- [Emotion](#emotion)

#### Face Smiling

| | ico | shortcode | ico | shortcode | |
| - | :-: | - | :-: | - | - |
| [top](#smileys--emotion) | :grinning: | `:grinning:` | :smiley: | `:smiley:` | [top](#table-of-contents) |
| [top](#smileys--emotion) | :smile: | `:smile:` | :grin: | `:grin:` | [top](#table-of-contents) |
| [top](#smileys--emotion) | :laughing: | `:laughing:` <br /> `:satisfied:` | :sweat_smile: | `:sweat_smile:` | [top](#table-of-contents) |
| [top](#smileys--emotion) | :rofl: | `:rofl:` | :joy: | `:joy:` | [top](#table-of-contents) |
| [top](#smileys--emotion) | :slightly_smiling_face: | `:slightly_smiling_face:` | :upside_down_face: | `:upside_down_face:` | [top](#table-of-contents) |
| [top](#smileys--emotion) | :wink: | `:wink:` | :blush: | `:blush:` | [top](#table-of-contents) |
| [top](#smileys--emotion) | :innocent: | `:innocent:` | | | [top](#table-of-contents) |

#### Face Affection

| | ico | shortcode | ico | shortcode | |
| - | :-: | - | :-: | - | - |
| [top](#smileys--emotion) | :smiling_face_with_three_hearts: | `:smiling_face_with_three_hearts:` | :heart_eyes: | `:heart_eyes:` | [top](#table-of-contents) |
| [top](#smileys--emotion) | :star_struck: | `:star_struck:` | :kissing_heart: | `:kissing_heart:` | [top](#table-of-contents) |
| [top](#smileys--emotion) | :kissing: | `:kissing:` | :relaxed: | `:relaxed:` | [top](#table-of-contents) |
| [top](#smileys--emotion) | :kissing_closed_eyes: | `:kissing_closed_eyes:` | :kissing_smiling_eyes: | `:kissing_smiling_eyes:` | [top](#table-of-contents) |
| [top](#smileys--emotion) | :smiling_face_with_tear: | `:smiling_face_with_tear:` | | | [top](#table-of-contents) |

#### Face Tongue

| | ico | shortcode | ico | shortcode | |
| - | :-: | - | :-: | - | - |
| [top](#smileys--emotion) | :yum: | `:yum:` | :stuck_out_tongue: | `:stuck_out_tongue:` | [top](#table-of-contents) |
| [top](#smileys--emotion) | :stuck_out_tongue_winking_eye: | `:stuck_out_tongue_winking_eye:` | :zany_face: | `:zany_face:` | [top](#table-of-contents) |
| [top](#smileys--emotion) | :stuck_out_tongue_closed_eyes: | `:stuck_out_tongue_closed_eyes:` | :money_mouth_face: | `:money_mouth_face:` | [top](#table-of-contents) |

#### Face Hand

| | ico | shortcode | ico | shortcode | |
| - | :-: | - | :-: | - | - |
| [top](#smileys--emotion) | :hugs: | `:hugs:` | :hand_over_mouth: | `:hand_over_mouth:` | [top](#table-of-contents) |
| [top](#smileys--emotion) | :shushing_face: | `:shushing_face:` | :thinking: | `:thinking:` | [top](#table-of-contents) |

#### Face Neutral Skeptical

| | ico | shortcode | ico | shortcode | |
| - | :-: | - | :-: | - | - |
| [top](#smileys--emotion) | :zipper_mouth_face: | `:zipper_mouth_face:` | :raised_eyebrow: | `:raised_eyebrow:` | [top](#table-of-contents) |
| [top](#smileys--emotion) | :neutral_face: | `:neutral_face:` | :expressionless: | `:expressionless:` | [top](#table-of-contents) |
| [top](#smileys--emotion) | :no_mouth: | `:no_mouth:` | :face_in_clouds: | `:face_in_clouds:` | [top](#table-of-contents) |
| [top](#smileys--emotion) | :smirk: | `:smirk:` | :unamused: | `:unamused:` | [top](#table-of-contents) |
| [top](#smileys--emotion) | :roll_eyes: | `:roll_eyes:` | :grimacing: | `:grimacing:` | [top](#table-of-contents) |
| [top](#smileys--emotion) | :face_exhaling: | `:face_exhaling:` | :lying_face: | `:lying_face:` | [top](#table-of-contents) |

#### Face Sleepy

| | ico | shortcode | ico | shortcode | |
| - | :-: | - | :-: | - | - |
| [top](#smileys--emotion) | :relieved: | `:relieved:` | :pensive: | `:pensive:` | [top](#table-of-contents) |
| [top](#smileys--emotion) | :sleepy: | `:sleepy:` | :drooling_face: | `:drooling_face:` | [top](#table-of-contents) |
| [top](#smileys--emotion) | :sleeping: | `:sleeping:` | | | [top](#table-of-contents) |

#### Face Unwell

