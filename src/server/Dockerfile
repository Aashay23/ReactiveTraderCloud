FROM microsoft/dotnet:2.0.0-sdk
WORKDIR /server

COPY ./*.sln ./NuGet.config  ./
COPY ./*/*.csproj ./
RUN for file in $(ls *.csproj); do mkdir -p ./${file%.*}/ && mv $file ./${file%.*}/; done
RUN dotnet restore
COPY . .