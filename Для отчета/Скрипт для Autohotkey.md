```
#Requires AutoHotkey v2.0

isWork := False

; Кнопкой F8 переключать работу авто подстановки машинного кода
F8::
{
  global isWork
  isWork := !isWork
}

; Цикл работы
Loop
{
  if (isWork)
  {
    Send "^1{Enter}" ; Посылает Ctrl 1 потом Enter
    Sleep 1500       ; Задержка в миллисекундах
  }
}

Numpad0::
{
  Send "^{Insert}" ; Посылает Ctrl Insert
  Send "{Enter}"   ; Посылает Enter
}

Esc::
{
  MsgBox "Конец работы скрипта"
  ExitApp ; Для завершения скрипта
}
```