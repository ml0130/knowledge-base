---
  title: Best Practices
---

--8<-- "includes/abbreviations.md"

When contributing to this project, aim to follow the best practices outlined below to ensure your changes are standardised and fit in with the existing format.

## File Names
Ensure new files are named lowercase only, so that the menu items are sorted alphabetically in a predictable way.

## Links
All links that navigate a user away from the site should have `{target=new}` appended - this opens the link in a new tab.

=== "Internal Link"

    ``` md
    [Internal Link](enroute.md)
    ```

=== "External Link"

    ``` md
    [External Link](https://vatpac.org){target=new}
    ```

!!! warning
    All external links should use the `https` protocol.

## Sector Names
Where available, controller positions and ARTCCs should be referred to by their abbreviation (e.g. SAN for Sydney Approach North, ZKC for Kansas City ARTCC) as well as other content you deem necessary.  Where multiple positions are discussed in close proximity, consider **bolding** the sector names.  The `abbreviations.md` file contains a list of all sector abbreivations and creates a tooltip with their full name for clarification.

## Altitudes
Describe any altitudes in the format of `Axxx` (for altitudes below 10,000ft) or `Fxxx` (for flight levels above 10,000ft) and wrap them in backticks.

!!! example
    ``` md
    Departures should climb to `A010`
    ```  
    Departures should climb to `A010`

## Radio Calls & Coordination
It is recommended to include an example highlighting any unique or lesser-known radio calls which apply to a procedure.

### Radio Calls
Radio calls should take the following format:  

``` md
**STATION NAME**: "Message"
```

!!! example
    **VOZ1545**: "VOZ1545, request descent"  
    **HUO**: "VOZ1545, descend to FL130" 

### Coordination
Coordination examples should take the following format:  

``` md
**INITIATING SECTOR** -> **RECEIVING SECTOR**: "Message"
```

!!! example
    **NW TCU** -> **WOL**: "Taxi, PSDN18 for YMCO via URBOB, Requesting F130"  
    **WOL** -> **NW TCU**: "PSDN18, F130"  
    **NW TCU** -> **WOL**: "F130, PSDN18" 

    **WOL** -> **NW TCU**: "via CB, SKJ, with your concurrence, will be assigned descent to A090"  
    **NW TCU** -> **WOL**: "SKJ, concur A090" 