# Then-return-
  endif     if (stringleft($tValue,1) &lt;> "}") then $tOutputLine= $tOutputLine &amp; " &amp; _ "      filewriteline($hFileOpen, $tOutputLine)     $i=$i+1 EndFunc  func getPosFirstNonWhiteSpace($str)     Local $aArray = StringToASCIIArray($str)      for $i=0 to ubound($aArray)-1         if $aArray[$i]&lt;>32 Then return $i     Next      return 0 EndFunc  func getInterfaceName()
