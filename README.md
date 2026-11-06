# PingBell

Digital signage on any TV, made in a chat.

PingBell turns what you tell your AI assistant into a board for the TV in your cafe, salon,
barbershop, gym, studio, clinic or office, and keeps it up to date. Describe what you want to
show: your menu and prices, your services and hours, today's class schedule, a sale with the
days left, holiday hours, Wi-Fi and guest info, an employee of the month, an announcement, or a
welcome screen with the time and weather. The assistant builds it from ready-made templates and
styles, with your words.

This repository is the PingBell plugin for Cursor, ChatGPT and other clients that read the
[Agent Plugin](https://agent-plugins.org) format. It connects to PingBell's hosted MCP server.
There is nothing to install or run locally.

## Connect

The server is `https://my.pingbell.io/mcp` (streamable HTTP). No sign-in or API key is needed.

**Cursor:** install PingBell from the Cursor Marketplace, or add it to `.cursor/mcp.json`:

```json
{
  "mcpServers": {
    "pingbell": {
      "url": "https://my.pingbell.io/mcp"
    }
  }
}
```

**Any other MCP client:** add a remote (streamable HTTP) server with the URL above.

## Try it

- "Make a menu for my cafe and put it on our TV"
- "Show our barbershop's services, prices and hours of operation on the TV"
- "Put today's class schedule on our fitness studio's TV"

## Put a board on a screen

Open the PingBell app on Fire TV, Roku, Apple TV or Android TV, or
[my.pingbell.io/pair](https://my.pingbell.io/pair) in any web browser. The screen shows a short
code: read it to your assistant, and the board appears right away. Ask for a change, like a new
price or today's special, and every screen updates by itself. You can also show a board on your
website.

Each board shows on up to 3 screens and carries a small "Powered by PingBell" mark.

## Tools

| Tool | What it does |
|---|---|
| `list_free_boards` | The boards that can be made, their lines, styles and backgrounds |
| `make_free_board` | Makes a board with your words |
| `get_free_board` | Reads a board back |
| `change_free_board` | Changes a board's words, style or background; every screen updates |
| `put_board_on_tv` | Shows a board on a screen, using the code the screen displays |
| `remove_board_from_tv` | Takes a board off a screen |
| `delete_free_board` | Deletes a board and everything stored with it |

## Your data

A board holds only the words you give it. You can delete a board and everything stored with it
at any time. See the [privacy policy](https://pingbell.io/privacy/) and
[terms](https://pingbell.io/terms/).

## Support

[pingbell.io/support](https://pingbell.io/support/) or support@pingbell.io.

## License

The plugin files in this repository are released under the MIT License. PingBell itself is a
hosted service, provided under its [terms](https://pingbell.io/terms/).
