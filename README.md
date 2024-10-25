<security>
      <authentication>
        <windowsAuthentication enabled="true" />
        <anonymousAuthentication enabled="true" />
      </authentication>
    </security>
    <location path="api/health">
      <system.webServer>
        <security>
          <authentication>
            <anonymousAuthentication enabled="true" />
            <windowsAuthentication enabled="false" />
          </authentication>
        </security>
      </system.webServer>
    </location>
    <location path="*">
      <system.webServer>
        <security>
          <authentication>
            <anonymousAuthentication enabled="false" />
            <windowsAuthentication enabled="true" />
          </authentication>
        </security>
      </system.webServer>
    </location>
