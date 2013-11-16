1. verify you have an LG screen

    ioreg -lw0 | grep IODisplayEDID | sed "/[^<]*</s///" | xxd -p -r | strings -6

    => LP133WP1-TJA3
       Color LCD

2. copy file to profiles

    sudo cp CustomMacRumors.icc /Library/ColorSync/Profiles/Displays

3. open system preferences / displays

4. select "color lcd"

5. done
