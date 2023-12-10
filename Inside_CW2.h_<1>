
#include <stdio.h>
#include <string.h>

typedef struct adventureGame{
    //look//
    const char* lookArray[13]; //arrays that contain the description of the each room

    //movement//
    const char* moveArray[13][4]; //arrays that contains all the possible direction user can move

    const int moveToArray[13][4]; //arrays that contains the room number that the user can move to in each direction
    const char* direction[4]; //arrays that contains all the direction user can move
    const char* dir[4]; //arrays that contains the short form of all the direction user can move

    //monster//
    const char* monsterArray[13]; //arrays that contains the name of the monster in each room
    const char* monsterShortFormKillCommandArray[13]; //arrays that contains the short form kill command of monster
    int monsterStatusArray[13]; //arrays that contains the status of the monster in each room
    int monsterHealthArray[13]; //arrays that contains the health of the monster in each room
    int monsterDamageArray[13]; //arrays that contains the damage of the monster in each room
    int monsterPreventionArray[13]; //arrays that contains the monster prevention status of each room
    int killMonsterXPArray[13]; //array of XP gained for killing respective monster in respective room

    //artifact//
    const int N_artifact; //number of artifact in the game
    const char* artifact[9]; //arrays that contains the name of the every artifact
    int artifactLoc[9]; //arrays that contains the location of the every artifact
    int getArtifactXPArray[9]; //array of XP gained for getting respective artifact
    int numArtifactsObtainedArray[9]; //arrays that contains the status of artifacts obtained by the player
    int artifactXPOnceFlag[9]; //arrays that contains the XP obtain status of each artifact
    const char* artifactHealingArray[9]; //arrays that contains the name of the artifact of heal type
    int artifactHealingEffectArray[9]; //arrays that contains the healing effect of the artifact of heal type

    //player//
    char name[1000]; // Allocate memory for the name of the player
    int playerHealth; //the health of the player
    int playerXP; //the XP player obtained by collecting artifacts and killing monsters
    int maxPlayerXP; //the maximum number of XP the player can get from the game
    int maxPlayerHealth; //the maximum health of the player
    int playerDamageArray[13]; //arrays that contains the damage of the player in each room

    //command//
    char command[1000]; // Allocate memory for the command from the user
    char lastCommand[1000]; //allocate memory for the last command entered by the user

    //inventory//
    int numItem; //the number of item in the inventory
    const int maxNumItem; //the maximum number of item the inventory can hold

    //attack//
    int swordDamageArray[13]; //arrays that contains the damage amplify effect of the sword in each room
    int diamondCrossDamageArray[13]; //arrays that contains the damage amplify effect of the diamond cross in each room
    int silverSpearDamageArray[13]; //arrays that contains the damage amplify effect of the silver spear in each room
    const char* artifactDamageArray[9]; //arrays that contains the name of the artifact of damage type

    //room//
    int room; //the current room number of the player
    int roomLockedArray[13]; //arrays that contains the lock status of each room
    char lockSymbolRoom10; //the symbol that represent the lock status of room 10 in map
    char lockSymbolRoom13; //the symbol that represent the lock status of room 13 in map
    const int bronzeKeyUnlockRoomNum; //the room number that the bronze key can unlock
    const int copperKeyUnlockRoomNum; //the room number that the copper key can unlock
    const char room1[1000]; //name of room in array element 0
    const char room2[1000]; //name of room in array element 1
    const char room3[1000]; //name of room in array element 2
    const char room4[1000]; //name of room in array element 3
    const char room5[1000]; //name of room in array element 4
    const char room6[1000]; //name of room in array element 5
    const char room7[1000]; //name of room in array element 6
    const char room8[1000]; //name of room in array element 7
    const char room9[1000]; //name of room in array element 8
    const char room10[1000]; //name of room in array element 9
    const char room11[1000]; //name of room in array element 10
    const char room12[1000]; //name of room in array element 11
    const char room13[1000]; //name of room in array element 12
} adventureGame;

//command//
void replaceNewLine(adventureGame *ag);
int processCommand(adventureGame *ag);
int processKillMonsterCommand(adventureGame *ag);

//movement//
int processMovement(adventureGame *ag);

//look//
void processLook(adventureGame *ag);

//monster//
int processKillMonster(adventureGame *ag);

//artifact//
int processGet(adventureGame *ag);
int processDrop(adventureGame *ag);
int processHealing(adventureGame *ag);
int addDamage(adventureGame *ag, int *i);
int minusDamage(adventureGame *ag, int *i);

//inventory//
int printInventory(adventureGame *ag);

//display information//
void printHelp(); //print the help menu
void printTips(adventureGame *ag); //print the function of each type of artifact
void printStatus(adventureGame *ag); //print the status of the player
void printScore(adventureGame *ag);
void printArtifactEffect(adventureGame *ag, int *i);
void displayProgressBar(adventureGame *ag);
void displayMonsterKilled(adventureGame *ag);
void displayArtifactObtained(adventureGame *ag);
void processMap(adventureGame *ag);

//room//
int processLockedDoor(adventureGame *ag);









