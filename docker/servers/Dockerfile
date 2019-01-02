FROM microsoft/dotnet
WORKDIR /app
COPY . .
RUN dotnet restore
CMD dotnet run -p Adaptive.ReactiveTrader.Server.Launcher all
