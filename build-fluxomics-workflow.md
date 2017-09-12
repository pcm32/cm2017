# Building a workflow

1. Go to https://public.phenomenal-h2020.eu/ and login with your email and password (if not registered, register through the PhenoMeNal Portal).

2. On the upper middle part (white over blue menus), click on "Workflow".

3. On the upper right, press on "Create new workflow".

4. Give the workflow a name: "Fluxomics exercise". Press "Create"

5. On the left hand side toolbar, under PHENOMENAL H2020, press on "Fluxomics".

6. **Adding nodes:** On the newly shown tools under Fluxomics, press on "ramid", then on "Iso2flux" and finally on "escher-fluxomics". As you press, you will notice that boxes get added to the canvas. Organize the boxes to follow the order in which they where added from left to right, top to bottom.

7. **Connecting nodes:**

   1. Use the blue rectangle to move the canvas to show the ramid box. Connect the output of ramid (outputExchange (csv)) to the input of midcor (input1).
   2. Connnect the only output of midcor to the "tracing data" input of Iso2flux.
   3. Connnect the "Best fit fluxes" output of Iso2flux to escher-fluxomics input with similar name.

8. Using the cog on the upper right, choose "Save".

9. Congratulations, you have created a workflow. To run the fluxomics workflow, you can follow the [Fluxomics Workflow Tutorial](https://portal.phenomenal-h2020.eu/help/fluxomics-workflow) at PhenoMeNal Portal.


