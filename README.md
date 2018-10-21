# Hi-there
def Poweset(L):
    if len(L) < 1:
       return [[]]
    small = Powerset(L[:-1])
    later = L[-1:]
    new = []
    for s in small:
        new.append(s + later)
    return small + new
