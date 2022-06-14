#### Mudblazer
##### manu
```cs
@using birdware.Shared.Account

<MudThemeProvider @bind-IsDarkMode="@_isDarkMode" Theme="CustomTheme" />
<MudDialogProvider />
<MudSnackbarProvider />

<MudLayout>
    <MudAppBar Elevation="1" Dense="true">
        <MudIconButton Icon="@Icons.Material.Filled.Menu" Color="Color.Primary" Edge="Edge.Start"
            OnClick="@((e) => DrawerToggle())" />

         <MudMenu FullWidth="true">
          <ActivatorContent>
          <MudChip Icon="" Color="Color.Primary">Contro</MudChip>
         </ActivatorContent>
     <ChildContent>
        <MudMenuItem>Profile</MudMenuItem>
        <MudMenuItem>Theme</MudMenuItem>
        <MudMenuItem>Usage</MudMenuItem>
        <MudMenuItem>Sign Out</MudMenuItem>
    </ChildContent>
        </MudMenu>

      <MudMenu FullWidth="true">
          <ActivatorContent>
          <MudChip Icon="" Color="Color.Primary">Home</MudChip>
         </ActivatorContent>
     <ChildContent>
        <MudMenuItem>Profile</MudMenuItem>
        <MudMenuItem>Theme</MudMenuItem>
        <MudMenuItem>Usage</MudMenuItem>
        <MudMenuItem>Sign Out</MudMenuItem>
    </ChildContent>
        </MudMenu>

        <MudMenu FullWidth="true">
          <ActivatorContent>
          <MudChip Icon="" Color="Color.Primary">Docs</MudChip>
         </ActivatorContent>
     <ChildContent>
        <MudMenuItem>Profile</MudMenuItem>
        <MudMenuItem>Theme</MudMenuItem>
        <MudMenuItem>Usage</MudMenuItem>
        <MudMenuItem>Sign Out</MudMenuItem>
    </ChildContent>
        </MudMenu>

        <MudMenu FullWidth="true">
          <ActivatorContent>
          <MudChip Icon="" Color="Color.Primary">App</MudChip>
         </ActivatorContent>
     <ChildContent>
        <MudMenuItem>Profile</MudMenuItem>
        <MudMenuItem>Theme</MudMenuItem>
        <MudMenuItem>Usage</MudMenuItem>
        <MudMenuItem>Sign Out</MudMenuItem>
    </ChildContent>
        </MudMenu>

        <MudSpacer />
        <MudIconButton Icon="@Icons.Custom.Brands.MudBlazor" Color="Color.Primary" Link="https://mudblazor.com/"
            Target="_blank" />

        <AccountDropDown/>
    </MudAppBar>
    <MudDrawer @bind-Open="@_drawerOpen" ClipMode="DrawerClipMode.Always" Elevation="1" justify-center
        Variant="@DrawerVariant.Mini" OpenMiniOnHover="true" Color="Color.Inherit">
        <MudSpacer />

        <NavMenu />

        <MudSpacer />
    </MudDrawer>
    <MudMainContent>

        <MudContainer MaxWidth="MaxWidth.Large" Class="my-16 pt-16">
        
            
            @Body
        </MudContainer>
    </MudMainContent>
</MudLayout>

@code {
    private bool _isDarkMode = false;
    bool _drawerOpen = false;
    bool open = false;
    MudTheme CustomTheme = new MudTheme()
    {
        Palette = new Palette()
        {
            Primary = Colors.Shades.Black,
            Secondary = Colors.Shades.White,
            AppbarBackground = Colors.Shades.White,
            DrawerBackground = Colors.Grey.Darken4,
        },
        PaletteDark = new Palette()
        {
            Primary = Colors.Blue.Lighten1
        },

        LayoutProperties = new LayoutProperties()
        {
            @* DrawerWidthLeft = "200px", *@
            @* DrawerWidthRight = "30px", *@
        }
    };
    void DrawerToggle()
    {
        _drawerOpen = !_drawerOpen;
    }
}

```
