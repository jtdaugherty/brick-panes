# Revision history for brick-panes

## 0.3.0.0 -- 2022-09-23

* Updated `handleFocusAndPanelEvents` to return a `PanelTransition` indication
  along with the new `Panel`.  This can be used by applications perform
  additional actions if the event just handled caused a transition into or out-of
  a modal Pane.

## 0.2.0.0 -- 2022-09-22

* Removed argument from `WhenFocusedModal` and
  `WhenFocusedModalHandlingAllEvents` `PaneFocus` constructors.  These arguments
  should always have been specified as `Nothing` by client code, with deleterious
  behavior if this requirement was not followed, so the need for this awkward
  constant representation was removed.

## 0.1.0.0 -- 2022-09-10

* Initial version.
