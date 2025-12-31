#include <stdio.h>

int car = 0, bike = 0, bus = 0;
int amount = 0, count = 0;

void menu();
void park();
void removeVehicle();
void showRecord();

int main()
{
    int choice;

    while (1)
    {
        menu();
        printf("\nEnter your choice: ");
        scanf("%d", &choice);

        switch (choice)
        {
        case 1:
            park();
            break;
        case 2:
            removeVehicle();
            break;
        case 3:
            showRecord();
            break;
        case 4:
            printf("\nThank you for using Parking System.\n");
            return 0;
        default:
            printf("\nInvalid choice! Try again.\n");
        }
    }
}

void menu()
{
    printf("\n===== VEHICLE PARKING MANAGEMENT SYSTEM =====");
    printf("\n1. Park Vehicle");
    printf("\n2. Remove Vehicle");
    printf("\n3. Show Parking Record");
    printf("\n4. Exit");
}

void park()
{
    int type;
    printf("\nEnter vehicle type:");
    printf("\n1. Car (Rs.50)");
    printf("\n2. Bike (Rs.20)");
    printf("\n3. Bus (Rs.100)");
    printf("\nEnter choice: ");
    scanf("%d", &type);

    if (type == 1)
    {
        car++;
        amount += 50;
        count++;
    }
    else if (type == 2)
    {
        bike++;
        amount += 20;
        count++;
    }
    else if (type == 3)
    {
        bus++;
        amount += 100;
        count++;
    }
    else
    {
        printf("\nInvalid vehicle type!\n");
    }
}

void removeVehicle()
{
    int type;
    printf("\nEnter vehicle type to remove:");
    printf("\n1. Car");
    printf("\n2. Bike");
    printf("\n3. Bus");
    printf("\nEnter choice: ");
    scanf("%d", &type);

    if (type == 1 && car > 0)
    {
        car--;
        amount -= 50;
        count--;
    }
    else if (type == 2 && bike > 0)
    {
        bike--;
        amount -= 20;
        count--;
    }
    else if (type == 3 && bus > 0)
    {
        bus--;
        amount -= 100;
        count--;
    }
    else
    {
        printf("\nNo vehicle of this type to remove!\n");
    }
}

void showRecord()
{
    printf("\n===== PARKING RECORD =====");
    printf("\nTotal Cars : %d", car);
    printf("\nTotal Bikes: %d", bike);
    printf("\nTotal Buses: %d", bus);
    printf("\nTotal Vehicles: %d", count);
    printf("\nTotal Amount Collected: Rs.%d\n", amount);
}
