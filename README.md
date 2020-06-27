# AshamaneCore-Fix (Bugtracker until upload)

**Instructions for removing procs from spells:
Add an entry to spell_proc (OR) spell_proc_event with the correct Spell ID with flags that don't make any sense for the current spell (such as adding demon hunter flag to a warrior spell).**

**Instructions for creating proc on specific aura:
Set proc flags for aura to all spell damage or all flags and then use p_ProcInfo from OnEffectProc in AuraScript to validate that the proc source is correct.**

_Notes:
Juggernaut currently uses spell_linked_spell and is not affected by spellscript other than to disable the aura proc._
