# Game  {if  putOnTop(Card card, Game game) {
  if (card.getOwnerId().equals(playerId)) {
    card.setZone(Zone.LIBRARY, game);
    library.addFirst(card.getId());
  } else {
    game.getPlayer(card.getOwnerId()).getLibrary().putOnTop(card, game);
  }  public void watch(GameEvent event, Game game) {
  if (event.getType() == GameEvent.EventType.MANA_PAID) {
    MageObject target = game.getObject(event.getTargetId());
    if (event.getSourceId() != null
        && event.getSourceId().equals(this.getSourceId()) && target != null && target.isCreature() && event.getFlag()) {
      if (target instanceof Spell) {
        this.creatures.add(((Spell) target).getCard().getId());
      } game.informplayers(message.toString());
	 
    } getObject() of mage.game.Game me.getState().setValue(source.getSourceId().toString() + "returnedCreature", new MageObjectReference(cardInGraveyard.getId(), game)); 

  }
}

}
