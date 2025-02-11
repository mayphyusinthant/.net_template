# .net_template
Initial Steps to develop web app using mvc.net & C# in Visual Studio Code 
✨ dotnet --list-sdks
✨ dotnet --list-runtimes
✨ dotnet --version
✨ Install C# extension
✨ Install ASP.NET Helper

✨ Create a new ASP.NET Core MVC project
	dotnet new mvc -n PetitionApp
	cd MyAspNetMvcApp

✨ Run The Project
	dotnet run
	dotnet project built and run on http://localhost:xxxx

✨ Make Changes in Razor View Model
	Project Folder > Views > Home > Index.cshtml
	Make some changes in contents and Link a html page inside the Index.cshtml
	HTML Files can be stored in Content Folder. 
	<a href="/Content/YourHtmlPage.html">New HTML Page</a>

✨ Configure Static File Serving in the program.cs
	using Microsoft.Extensions.FileProviders;
	app.UseStaticFiles();

	app.UseStaticFiles(new StaticFileOptions
	{
    		FileProvider = new PhysicalFileProvider(Path.Combine(Directory.GetCurrentDirectory(), "Content")),
    		RequestPath = "/Content"
	});

Additional Tips:
Use the dotnet build and dotnet watch run commands for efficient development.
Ensure that launch.json and tasks.json files in the .vscode directory are properly configured for debugging if required.
Noted by May.
