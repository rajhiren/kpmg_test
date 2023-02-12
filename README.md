# KPMG Python test for Texas Hold'em Poker


## Prerequesites
```
pip install -r requirements.xtx
```

## Usage
Run the main program in debug mode to see all the player hands.

```
usage: python3 main.py [-h] -c COMMUNITY -p PLAYER -d DEBUG
python3 main.py: error: the following arguments are required: -c/--community, -p/--player, -d/--debug
  
```

Run the main program to see the required two cards to make the selected winner.

```
Example:

python3 main.py -d 1 -p David  -c  S10,DA,CJ 

------------------------------ Debugging Mode On ------------------------------

It took 1 iterations to find the required cards 
Winner: David
Cards:
All Community cards: 	 [S10] (S9, SJ)
____________________________________________________________________________________________________
Player    |Card in Hand        |Hands                         |Hand Type           |Hand Ranking
____________________________________________________________________________________________________
John      |[H2, C8]            |[H2, C8, S9, S10, SJ]         |High Card           |       140
David     |[Sk, Sq]            |[S9, S10, SJ, Sq, Sk]         |Straight Flush      |       955
Siva      |[Ca, D7]            |[D7, S9, S10, SJ, Ca]         |High Card           |       151
Raj       |[H9, Dk]            |[S9, H9, S10, SJ, Dk]         |Pair                |       252
Mahi      |[S5, D3]            |[D3, S5, S9, S10, SJ]         |High Card           |       138
test      |[D9, S8]            |[S8, S9, D9, S10, SJ]         |Pair                |       247
data      |[Ck, Cq]            |[S9, S10, SJ, Cq, Ck]         |Straight            |       555
____________________________________________________________________________________________________
Required Cards: (S9, SJ)


((S9, SJ), 1, 1)

```

## More about Texas Holde'm Poker
[Texas Holde'm Wikipedia](https://en.wikipedia.org/wiki/Texas_hold_%27em)

## Things To Do
```
    1. Add Tests
    2. Add to Docker Container
    3. Add Some UI
    4. Can use AI tool or rewrite using `poker` library
```