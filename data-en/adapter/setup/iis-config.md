# IIS Setup

## Application Pools

It is required to create a new application pool in the IIS service manager that will work with the *Loginom Adapter* It is possible to run the IIS service manager by the `inetmgr` command using the **Run** menu.

Then the ** IIS service manager ** window will appear. A new application pool needs to be created in the **IIS service manager**. This task is possible by using the **Add Application Pool…** (*Add Application Pool…*) item in the context menu of the **Application Pools** (*Application Pools*) element.

In the **Application Pool Addition** window that appears, it is required to set the values of the following parameters: the pool **name** for the *Adapter*, for example, `LoginomAdapterAppPool`, to specify **CLR environment version. NET**, to set the **controlled conveyer mode** — embedded.

> **Note**: when the *Loginom Integrator* and *Loginom Adapter* are used on the one IIS server, different application pools must be set for them.

To view/change the application list, it is required to select **View applications** in the context menu of the selected pool.

## Special Login Account

It is required to configure the additional parameters (for example, using the following menu item: **Set Application Pool Defaults…** (*Set Application Pool Defaults…*) in the created application pool. In the opened window for the **Identity** (*Identity*) parameter, it is required to set the pre-created special login account of the application pool with the [required rights](./special-user.md#neobkhodimye-prava) essential for the *Adapter* operation.
