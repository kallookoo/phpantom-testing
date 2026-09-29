# phpantom-testing


## Current Zed Settings

```json
// Zed settings
//
// For information on how to configure Zed, see the Zed
// documentation: https://zed.dev/docs/configuring-zed
//
// To see all of Zed's default settings without changing your
// custom settings, run `zed: open default settings` from the
// command palette (cmd-shift-p / ctrl-shift-p)
{
  // "proxy": "http://127.0.0.1:8080",
  "agent": {
    "default_profile": "ask",
    "default_model": {
      "provider": "********", // Edited for privacy
      "model": "********", // Edited for privacy
      "enable_thinking": true,
    },
    "favorite_models": [],
    "model_parameters": [],
  },
  "file_types": {
    "Ghostty": ["**/ghostty/config"],
  },
  "agent_servers": {
    "oc": {
      "favorite_config_option_values": {
        "model": ["********"], // Edited for privacy
      },
      "default_config_options": {
        "effort": "max",
        "mode": "plan",
        "model": "********", // Edited for privacy
      },
      "type": "custom",
      "command": "/Users/sergio/.opencode/bin/opencode",
      "args": ["acp"],
    },
  },
  "wrap_guides": [80, 100, 120],
  // "buffer_font_features": {
  //   "calt": true,
  //   "liga": true,
  //   "ss01": true,
  //   "ss02": true,
  //   "ss03": true,
  //   "ss04": true,
  //   "ss05": true,
  //   "ss06": true,
  //   "ss07": true,
  //   "ss08": true,
  //   "ss09": true,
  //   "ss10": true,
  //   "cv01": 2,
  //   "cv02": 1,
  //   "cv31": true,
  //   "cv32": true,
  //   "cv62": true,
  // },
  "title_bar": {
    "show_user_menu": false,
    "show_sign_in": false,
    "show_branch_status_icon": true,
  },
  "status_bar": {
    "line_endings_button": true,
  },
  "theme": {
    "mode": "system",
    "light": "One Dark",
    "dark": "One Dark",
  },
  "redact_private_values": true,
  "cli_default_open_behavior": "new_window",
  "show_edit_predictions": false,
  "close_on_file_delete": true,
  "icon_theme": "Material Icon Theme",
  "collaboration_panel": {
    "button": false,
  },
  "edit_predictions": {
    "provider": "none", // none, remove icon.
    "allow_data_collection": "no",
  },
  "format_on_save": "off",
  "languages": {
    "Swift": {
      "language_servers": ["sourcekit-lsp", "package-swift-lsp"],
    },
    "PHP": {
      "language_servers": [
        "phpantom",
        "!intelephense",
        "!phpactor",
        "!phptools",
        "...",
      ],
      "formatter": "language_server",
      "format_on_save": "on",
    },
    "JavaScript": {
      "code_actions_on_format": {
        "source.fixAll.eslint": true,
      },
    },
    "TypeScript": {
      "code_actions_on_format": {
        "source.fixAll.eslint": true,
      },
    },
  },
  "lsp": {
    "json-language-server": {
      "settings": {
        "json": {
          "schemas": [
            {
              "fileMatch": ["composer.json"],
              "url": "https://getcomposer.org/schema.json",
            },
          ],
        },
      },
    },
    "vtsls": {
      "settings": {
        "typescript": {
          "updateImportsOnFileMove": {
            "enabled": "always",
          },
        },
        "javascript": {
          "updateImportsOnFileMove": {
            "enabled": "always",
          },
        },
      },
    },
    "eslint": {
      "settings": {
        "useFlatConfig": true,
      },
    },
    "tailwindcss-language-server": {
      "settings": {
        "includeLanguages": {
          "php": "html",
          "blade": "html",
        },
        "experimental": {
          "classRegex": [
            // PHP/Lavarel
            "class=\"([^\"]*)\"",
            "class='([^']*)'",
            "class=\\\"([^\\\"]*)\\\"",
            "@class\\(\\[([^\\]]*)\\]\\)",
            // TS/JS
            "\\.className\\s*[+]?=\\s*['\"]([^'\"]*)['\"]",
            "\\.setAttributeNS\\(.*,\\s*['\"]class['\"],\\s*['\"]([^'\"]*)['\"]",
            "\\.setAttribute\\(['\"]class['\"],\\s*['\"]([^'\"]*)['\"]",
            "\\.classList\\.add\\(['\"]([^'\"]*)['\"]",
            "\\.classList\\.remove\\(['\"]([^'\"]*)['\"]",
            "\\.classList\\.toggle\\(['\"]([^'\"]*)['\"]",
            "\\.classList\\.contains\\(['\"]([^'\"]*)['\"]",
            "\\.classList\\.replace\\(\\s*['\"]([^'\"]*)['\"]",
            "\\.classList\\.replace\\([^,)]+,\\s*['\"]([^'\"]*)['\"]",
          ],
        },
      },
    },
  },
  "minimap": {
    "show": "always",
  },
  "telemetry": {
    "diagnostics": false,
    "metrics": false,
  },
  "terminal": {
    "shell": "system",
    "working_directory": "current_file_directory",
  },
}
```

## Current Global Composer

```json
{
	"config": {
		"allow-plugins": {
			"dealerdirect/phpcodesniffer-composer-installer": true
		}
	},
	"require-dev": {
		"kallookoo/phpcs-rules": "^1.0"
	}
}

```
