while True:                    #cyklus, který bude probíhat pořád
    cislo = input("Zadejte číslo")
    if cislo.lstrip("-").isdigit():
        max = int(cislo)
        break
    else:
        print("Nezadali jste číslo")
while input("Pro ukončení zadejte písmeno K") != "K":
    cislo = input("Zadejte číslo: ")
    if cislo.isdigit():
        cislo = int(cislo)
        if max < cislo:
            max = cislo
    else:
        print("Nezadali jste číslo")
print("Největší číslo bylo: " + str(max))
