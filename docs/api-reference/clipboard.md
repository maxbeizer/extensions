# Clipboard

## Overview

You can write contents to the clipboard through {@link writeTextToClipboard} and clear it through [clearClipboard](file:///Users/mann/Developer/api-alpha/documentation/modules.html#clearClipboard). We also provide convenience actions such as [CopyToClipboardAction](file:///Users/mann/Developer/api-alpha/documentation/modules.html#CopyToClipboardAction) or [OpenInBrowserAction](file:///Users/mann/Developer/api-alpha/documentation/modules.html#OpenInBrowserAction) for standard [ActionPanel](file:///Users/mann/Developer/api-alpha/documentation/modules.html#ActionPanel)operations.

## API Reference

### clearClipboard

Clears the current clipboard contents.

#### Signature

```typescript
async function clearClipboard(): Promise<void>
```

#### Return

A promise that resolves when the clipboard is cleared.

### copyTextToClipboard

Copies text to the clipboard.

#### Signature

```typescript
async function copyTextToClipboard(text: string): Promise<void>
```

#### Parameters

| Name | Type | Required | Description |
| :--- | :--- | :--- | :--- |
| text | `string` | Yes |  |

#### Return

A promise that resolves when the text got copied to the clipboard.

### getSelectedText

Gets the selected text of the frontmost application.

#### Signature

```typescript
async function getSelectedText(): Promise<string>
```

#### Return

Returns a promise that resolves with the selected text.

### pasteText

Pastes text to the current selection of the frontmost application.

#### Signature

```typescript
async function pasteText(text: string): Promise<void>
```

#### Parameters

| Name | Type | Required | Description |
| :--- | :--- | :--- | :--- |
| text | `string` | Yes | The text contents to insert at the cursor. |

#### Return

A promise that resolves when the text got pasted.