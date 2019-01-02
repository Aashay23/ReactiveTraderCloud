FROM microsoft/dotnet:latest
WORKDIR /app
COPY . .
RUN dotnet restore
RUN dotnet run -p Adaptive.ReactiveTrader.Server.Launcher --populate-eventstore
CMD dotnet run -p Adaptive.ReactiveTrader.Server.Launcher all