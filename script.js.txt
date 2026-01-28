let count = 0;

function cardCounter(card) {
  if (card >= 2 && card <= 10) {
    if (card >= 2 && card <= 6) {
      count++;
    } else if (card >= 7 && card <= 9) {
    } else if (card === 10) {
      count--;
    }
  } else if (card === 'A' || card === 'J' || card === 'Q' || card === 'K') {
    count--;
  }

  if (count > 0) {
    return count + " Bet";
  } else {
    return count + " Hold";
  }
}