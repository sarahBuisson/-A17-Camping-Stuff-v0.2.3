# -A17-Camping-Stuff-v0.2.3
Nandonalt's Camping Stuff v0.2.3 updated to a17
Sourced from steam with the following changes:

Removed the references to Microsoft.CSharp and System.Net.Http and setting .net target to 3.5 (these may just be my visual studio adding stuff on me)
Changed 'stringToLines' to 'StringToLines' on CompTargetable_Tent.cs lines 53 & 195
Changed 'getPlacements' to 'GetPlacements' on CompTargetable_Tent.cs lines 191, 306, & 530 and CompPackTents.cs line 93
Added a '-1,' to CompTargetable_Tent.cs line 446 so it reads: return GenClosest.ClosestThingReachable(pawn.Position, pawn.Map, ThingRequest.ForDef(this.parent.Stuff), PathEndMode.InteractionCell, TraverseParms.For(pawn, pawn.NormalMaxDanger(), TraverseMode.ByPawn, false), 9999f, validator, null, -1, -1, false);
Changed 'Scribe_Values.LookValue' to 'Scribe_Values.Look' on CompPackTent.cs lines 64 & 65
Deleted CompPackTent.cs lines 179-204
Changed CompPackTent.cs lines 153-164 to:
  nodoor = false;
  thingList2[i].Destroy(DestroyMode.Vanish);

Unsure of licenseing info, as Nandonalt didn't originally publish anything in that respect.

To install a non-workshop Rimworld mod:
1. Go to your RimWorld install folder (by windows default its C:\Program Files (x86)\Steam\steamapps\common\RimWorld) and open the "Mods" folder.
2. Copy the "Nandonalt_CampingStuff-a17" folder from the zip to the Mods folder (DO NOT put it inside Core)
3. After that run Rimworld and "Camping Stuff" will show up in your mod list (again) with a little folder icon next to it.
4. From there it should be just like anyother workshop item
