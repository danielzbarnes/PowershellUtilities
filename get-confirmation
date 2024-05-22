# simple function to get a Yes/No response
function Get-Confirmation{

    [cmdletbinding()]
    param(
        [Parameter(Mandatory=$true)]
        [ValidateNotNullOrEmpty()]
        [string]$Prompt
    )

    while($true){    
        $input = Read-Host -Prompt $Prompt

        if ($input -eq 'y') {
            return $true
        } elseif ($input -eq 'n'){
            return $false
        } else {
            Write-Host "Please enter a valid selection." -ForegroundColor Red
        }
    }
}
