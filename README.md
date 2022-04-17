# -SetError
 If BitAND($dFlag, 8) = 8 Then $sAlphaEx &amp;= "_" ; Include Underscore      $aWordArray = StringRegExp($sString, "[" &amp; $sAlphaEx &amp; "]+", 3) ; Split into words     If Not @error Then         SetExtended(UBound($aWordArray)) ; Set the extended flag to the number of words found         Return $aWordArray     EndIf      Return SetError(3, 0, 0) ; No matches found EndFunc
