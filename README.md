
paquete quicksort

func  QuickSort ( slice [] int ) {
  rápido (slice, 0 , len (slice) - 1 )
}

func  quick ( slice [] int , start  int , end  int ) {
  if start <end {
    pivotIndex  : =  división (corte, inicio, fin)
    rápido (slice, start, pivotIndex- 1 )
    rápido (slice, pivotIndex + 1 , final)
  }
}

func  split ( slice [] int , start  int , end  int ) int {
  pivot  : = slice [end]
  j  : = inicio

  para  índice  : = inicio; índice <fin; índice ++ {
    if slice [index] <pivot {
      temp  : = slice [index]
      slice [index] = slice [j]
      slice [j] = temp
      j = j + 1
    }
  }

  si pivot <= slice [j] {
    slice [end] = slice [j]
    rebanada [j] = pivote
  }
  
  devolver j
}
