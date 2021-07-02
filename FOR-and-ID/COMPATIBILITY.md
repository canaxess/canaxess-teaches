# Compatibility
This matrix describes the actual output behaviour between screen readers and browsers.

Test = `label created by FOR and ID attributes announced by screen reader`

|                      | NVDA 2020 | JAWS 2021 | VoiceOver | TalkBack 9.1 | Voice Assistant |
|----------------------|:---------:|:---------:|:---------:|:------------:|:---------------:|
| Chrome 91            | yes         | *         | n/a         | n/a            | n/a               |
| Firefox 88           | *         | *         | n/a         | n/a            | n/a               |
| Edge (Chromium) 91   | yes         | *         | n/a         | n/a            | n/a               |
| Internet Explorer 11 | yes        | *         | n/a         | n/a            | n/a               |
| Safari iOS 14.3      | n/a         | n/a         | yes         | n/a            | n/a               |
| Chrome Android 10    | n/a         | n/a         | n/a         | yes            | yes               |

## Screen reader output

- Talkback = `"edit box enter your name"`
- Voice Assistant = `"edit box enter your name"`
- VoiceOver = `"enter your name text field"`
- NVDA `"enter your name edit blank"`
