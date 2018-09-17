1)dotnet new mvc
2)<PackageReference Include="Microsoft.VisualStudio.Web.CodeGeneration.Design" Version="2.0.0" />  
   and
   <DotNetCliToolReference Include="Microsoft.EntityFrameworkCore.Tools.DotNet" Version="2.0.0" />
3) dotnet restore 
4)dotnet ef dbcontext scaffold "Server=abhay;Database=EFCoreDBFirstDemo;Trusted_Connection=True;User Id=sa;Password=abhay;Integrated Security=false;" Microsoft.EntityFrameworkCore.SqlServer -o Models/DB
5)dotnet aspnet-codegenerator controller -name StudentController -m Student -dc EFCoreDBFirstDemoContext --relativeFolderPath Controllers --useDefaultLayout --referenceScriptLibraries