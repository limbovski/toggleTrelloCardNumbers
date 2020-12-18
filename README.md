# toggleTrelloCardNumbers
Bookmarklet to toggle the display of card numbers for cards on a Trello board


javascript:(function(){$(".card-short-id").each(function(){    let card = $(this);      let newCardText = card.text();         newCardText = newCardText.replace("#","");    newCardText += " ";        card.text(newCardText);    $(this).hasClass("hide")?$(this).removeClass("hide"):$(this).addClass("hide");});})()
