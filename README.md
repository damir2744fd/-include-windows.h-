# -include-windows.h-
If Not @AutoItX64 Then     Local $Code = '...'     Local $Reloc = '...'     Local $Symbol[] = ["main"]      Local $CodeBase = _BinaryCall_Create($Code, $Reloc)     If @Error Then Exit      Local $SymbolList = _BinaryCall_SymbolList($CodeBase, $Symbol)     If @Error Then Exit EndIf
